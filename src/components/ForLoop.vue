<template>
  <div>
    <h1>For Loop in Vue Js</h1>
    <table class="styled-table">
      <thead>
        <tr>
          <th>ID</th>
          <th>NAME</th>
          <th>EMAIL</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="user in users" :key="user.id">
          <td>{{ user.id }}</td>
          <td>{{ user.name }}</td>
          <td>{{ user.email }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "ForLoop",
  data() {
    return {
      users: [
        { id: 1, name: "peter", email: "peter@test.com" },
        { id: 2, name: "sam", email: "sam@test.com" },
        { id: 3, name: "tony", email: "tony@test.com" },
        { id: 4, name: "champ", email: "champ@test.com" },
        { id: 5, name: "bruce", email: "bruce@test.com" },
      ],
    };
  },
};
</script>

<style>
.styled-table {
    border-collapse: collapse;
    margin: 25px 0 0 525px;
    font-size: 0.9em;
    font-family: sans-serif;
    min-width: 400px;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
}

.styled-table thead tr {
    background-color: #009879;
    color: #ffffff;
    text-align: left;
}
.styled-table th,
.styled-table td {
    padding: 12px 15px;
}

.styled-table tbody tr {
    border-bottom: 1px solid #dddddd;
}

.styled-table tbody tr:nth-of-type(even) {
    background-color: #f3f3f3;
}

.styled-table tbody tr:last-of-type {
    border-bottom: 2px solid #009879;
}
.styled-table tbody tr.active-row {
    font-weight: bold;
    color: #009879;
}
</style>