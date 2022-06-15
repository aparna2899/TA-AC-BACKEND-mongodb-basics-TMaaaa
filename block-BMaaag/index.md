writeCode

Write code to:-

- create a database named `mountains`
- a collection inside that database named `himalayas`
- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`

- insert multiple document using insertMany command
- find all documents from mountains
- find a single document using name

use mountains

db.himalayas.insertMany([{name: 'Nanga Parbat',height: '8126 mtrs'},{name: 'Namjagbarwa','height: '7756 mtrs'},{name:'Kanchenjunga',height:'8586 mtrs'},{name:'Nanda Devi',height:'7816'}])

db.himalayas.insert(ranges)

db.himalayas.find()

db.himalayas.find({name:'Nanda Devi'})
