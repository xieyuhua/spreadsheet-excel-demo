# spreadsheet-excel-demo

### example
```
<body >
  <div id="wrapper"></div>
  <script>
        window.onload = function () {
              DaView = localStorage.getItem('keysasas');
              DaView = JSON.parse(DaView)
              xspreadsheet(document.getElementById('wrapper')).loadData((DaView)).change(function (data) {
                    console.log('data:', JSON.stringify(data))
                    localStorage.setItem('keysasas', JSON.stringify(data));
              });
        }
  </script>
<script type="text/javascript" src="xspreadsheet.js"></script>
</body>
```


### spreadsheet-excel 效果图

![image](https://user-images.githubusercontent.com/29120060/194519458-b9c11cb4-5d55-4968-b969-db5cc1c0219a.png)

![image](https://user-images.githubusercontent.com/29120060/194519527-e512676d-7b29-435a-b5aa-3ec83c7a46e1.png)
