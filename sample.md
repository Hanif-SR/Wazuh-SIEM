<ossec_config>
  <client>
    <server>
      <address>192.168.100.227</address>
    </server>

    <!-- System logs -->
    <localfile>
      <log_format>syslog</log_format>
      <location>/var/log/syslog</location>
    </localfile>

    <localfile>
      <log_format>syslog</log_format>
      <location>/var/log/auth.log</location>
    </localfile>

    <!-- Nginx logs -->
    <localfile>
      <log_format>syslog</log_format>
      <location>/var/log/nginx/access.log</location>
    </localfile>

    <localfile>
      <log_format>syslog</log_format>
      <location>/var/log/nginx/error.log</location>
    </localfile>

    <!-- Node.js logs -->
    <localfile>
      <log_format>syslog</log_format>
      <location>/var/log/node-app.log</location>
    </localfile>
  </client>
</ossec_config>
