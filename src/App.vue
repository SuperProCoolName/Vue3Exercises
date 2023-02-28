<script>
export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: "name1",
          salary: 100,
          age: 30,
          isEdit: false,
        },
        {
          id: 2,
          name: "name2",
          salary: 200,
          age: 40,
          isEdit: false,
        },
        {
          id: 3,
          name: "name3",
          salary: 300,
          age: 50,
          isEdit: false,
        },
      ],
    };
  },
  methods: {
    removeItem: function (id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;
      });
    },
    edit: function (user) {
      user.isEdit = true;
    },
    save: function (user) {
      user.isEdit = false;
    },
  },
};
</script>
<template>
  <table>
    <tr>
      <th>Id</th>
      <th>Name</th>
      <th>Salary</th>
      <th>Age</th>
    </tr>
    <tr v-for="user in users">
      <template v-if="!user.isEdit">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.salary }}</td>
        <td>{{ user.age }}</td>
        <td><button @click="removeItem(user.id)">remove</button></td>
        <td><button @click="edit(user)">edit</button></td>
      </template>
      <template v-else>
        <td><input v-model="user.id" /></td>
        <td><input v-model="user.name" /></td>
        <td><input v-model="user.salary" /></td>
        <td><input v-model="user.age" /></td>
        <td><button @click="save(user)">save</button></td>
      </template>
    </tr>
  </table>
</template>
