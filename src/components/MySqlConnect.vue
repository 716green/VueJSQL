<template>
  <div class="mysql-connect">
    <h2>{{items.pageName}} Component</h2>
    <h2>MySQL Connector for {{ items.ipAddress }}</h2>
    <!--
      Saved as an example:
      If ip address exists, show. Then iterate through each item in items (server details) with a separate p tag
    -->
    <div v-show="(items.ipAddress.length > 0)">
      <ul>
        <li v-for="item in items">{{item}}</li>
        <!--:key="items.ipAddress"-->
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      name: "MyJSQL",
      items: {
        database: "MySQL",
        serverName: "My Server",
        ipAddress: "123.456.7.890",
        userName: "root",
        password: "Ashland123", //move to .env?
        frontEnd: "VueJS",
        pageName: "MySqlConnect"
      }
    };
  }
};
</script>

<style>
.mysql-connect {
  color: darkolivegreen;
  font-family: "Courier New", Courier, monospace;
  font-weight: bolder;
  text-align: left;
  align-content: left;
}
</style>
