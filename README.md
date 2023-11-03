# server.js
const motoGP = [
    {
      "circuit": "Losail",
      "location": "Qatar",
      "winner": {
        "firstName": "Andrea",
        "lastName": "Dovizioso",
        "country": "Italy"
      }
    },
    {
      "circuit": "Autodromo Termas de Rio Hondo",
      "location": "Argentina",
      "winner": {
        "firstName": "Cal",
        "lastName": "Crutchlow",
        "country": "UK"
      }
    },
    {
      "circuit": "Circuito de Jerez - Ángel Nieto",
      "location": "Spain",
      "winner": {
        "firstName": "Valentino",
        "lastName": "Rossi",
        "country": "Italy"
      }
    },
    {
      "circuit": "Mugello",
      "location": "Italy",
      "winner": {
        "firstName": "Andrea",
        "lastName": "Dovizioso",
        "country": "Italy"
      }
    }
  ];
  
  
  const express = require("express");
  const app = express();
  
 
  app.get(`/`, (req, res) => {
    
    res.send(JSON.stringify(motoGP));
  });
  app.listen(5000, () => console.log(`Server Berjalan di http://localhost:5000`));
  //Nama:Andika Rizky H
  //Kelas:TI 22J
