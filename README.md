
# Express1stlyCreatedThings

const port = 5000;
.
.

const express = require("express");
var cors = require("cors");

const app = express();
app.use(cors());
app.use(express.json());



.
.
.


app.get("/", (req, res) => {
  res.send(dv);
});


.
.
.
.




app.get("/user", (req, res) => {
  console.log("query", req.query);
  res.send(dv);
});


app.get("/user/:id", (req, res) => {
  let id = +req.params.id;
  console.log(typeof id);

  const value = dv.filter((v) => v.value == id);
  console.log("value", value);

  if (id <= 4) {
    res.send(value);
  } else {
    res.send("ses Yr..");
  }
});



.
.
.



app.listen(port, () => {
  console.log("port running");
});

.
.
.

# ROUTER EXPRESS 😝

😮‍ const express = require('express') 

😮‍💨 const adminRouter = express.Router()

# last e 🥇
😮‍💨 module.exports = adminRouter

# main e router implement 🥈

😮‍💨 const adminRouter = require('./adminRoute')

😮‍💨 app.use('/admin',adminRouter)




