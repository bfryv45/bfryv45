fetch('https://api.gofile.io/servers', {
  method: 'GET'
})
.then(response => response.json())
.then(data => {
  console.log(data);
})
.catch(error => console.error(error));
{
  "status": "ok",
  "data": {
    "servers": [
      {"name":"store1","zone":"eu"},
      {"name":"store3","zone":"na"}
    ]
  }
}
*
fetch('https://api.gofile.io/contents/a3fbf37e-36f5-4d91-b2c8-fe4b250979b7/directlinks', {
  method: 'POST',
  headers: {
    'Authorization': 'Bearer your_token_here'
  }
})
.then(response => response.json())
.then(data => console.log(data))
.catch((error) => {
  console.error('Error:', error);
});3
