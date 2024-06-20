<!DOCTYPE html>
<html>
<head>
  <title>TCP File Uploader</title>
</head>
<body>
  <h1>TCP File Uploader</h1>
  <input type="file" id="fileInput" />
  <button id="uploadButton">Upload File</button>
  <div id="status"></div>

  <script>
    const fileInput = document.getElementById('fileInput');
    const uploadButton = document.getElementById('uploadButton');
    const statusDiv = document.getElementById('status');

    uploadButton.addEventListener('click', () => {
      const file = fileInput.files[0];
      const socket = new WebSocket('ws://localhost:7070');

      socket.onopen = () => {
        console.log('Connected to server');

        const reader = new FileReader();
        reader.onload = () => {
          const fileBuffer = reader.result;
          socket.send(fileBuffer);
          statusDiv.innerHTML = 'File uploaded successfully!';
        };

        reader.readAsArrayBuffer(file);
      };

      socket.onerror = (err) => {
        console.log('Error: ' + err);
        statusDiv.innerHTML = 'Error uploading file: ' + err;
      };

      socket.onclose = () => {
        console.log('Disconnected from server');
      };
    });
  </script>
</body>
</html>
