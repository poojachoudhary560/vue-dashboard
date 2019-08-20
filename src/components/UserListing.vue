<template>
  <v-data-table :headers="headers" :items="userlist">
    <template v-slot:headers="props">
      <tr>
        <th v-for="header in props.headers" :key="header.text">{{header.text}}</th>
      </tr>
    </template>
    <template v-slot:items="props">
      <td class="text-xs-right">{{props.item.username}}</td>
      <td class="text-xs-right">{{props.item.email}}</td>
      <td class="text-xs-right">{{props.item.department}}</td>
    </template>
  </v-data-table>
</template>
<script>
export default {
  data() {
    return {
      headers: [
        {
          text: "Username",
          value: "username"
        },
        {
          text: "Email",
          value: "email"
        },
        {
          text: "Department",
          value: "department"
        }
      ],
      userlist: [
        {
          username: "sample name",
          email: "sample.name@example.com",
          department: "test 1"
        },
        {
          username: "sample name1",
          email: "sample.name1@example.com",
          department: "test 2"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>
