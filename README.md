# hoodieshop
[How Hood.ie works](http://docs.hood.ie/en/latest/about/how-hoodie-works.html)
[Glossary](http://docs.hood.ie/en/latest/about/glossary.html)

### introduction
```
mkdir init
cd init
npm init
npm install hoodie --save
edit package.json >> scripts.start = "hoodie"
npm start
go to http://127.0.0.1:8080/hoodie/store/
open console 
type hoodie
yay!
some secrets http://127.0.0.1:8080/hoodie/admin/
```

```
add this to package.json
  "hoodie": {
    "address": "127.0.0.1",
    "port": 8080,
    "data": ".hoodie",
    "public": "public",
    "dbUrl": "",
    "dbAdapter": "pouchdb-adapter-fs",
    "inMemory": false,
    "loglevel": "warn",
    "url": "",
    "adminPassword": "secret"
  }
```

```
hoodie.store.add({name: 'grey'})
hoodie.store.findAll().then(console.table)
hoodie.store.update({_id: '8AC219A6-312C-0F8E-AC0D-1CEE73D84D50', name: 'red'})
hoodie.store.remove({_id: '8AC219A6-312C-0F8E-AC0D-1CEE73D84D50'})
```
### configuration

http://docs.hood.ie/en/latest/guides/configuration.html

### Based on Hoodie

https://tracker.hood.ie/
https://minutes.io/welcome
https://github.com/hoodiehq/hoodie-app-mapchat

### plugins
[lot of plugins](https://www.npmjs.com/search?q=hoodie-plugin-)
