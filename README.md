# server-site--basic-stacture

const express = require('express');
const cors = require('cors');
const app = express();
const port = process.env.PORT || 5000;


// maidware 

app.use(cors());
app.use(express.json());


app.get("/",( req, res)=>{
    
    res.send("e_commarce sit ")
})

app.listen( port, ()=>{
    console.log(` e_commarce site is running ${port}`);
});

