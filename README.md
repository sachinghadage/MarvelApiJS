// My Public API - a626b5aa437ad6f953dd6a8460cf1096
// MD5 Hash - 6d5b79bca2f0244f4c207aef2cd8cd30


//generate hash key throw api.js file which is given below
// first install crypto-js
// npm install crypto-js
// now use md5 as below
// var MD5 = require("crypto-js/md5"); 
// console.log(MD5("text to hash").toString());

var CryptoJS = require("crypto-js");

// Replace with your timestamp, private key, and public key
var ts = "1"; // Example timestamp
var privateKey = "4f8b75d2c7488b0b4095a8dd7d4bc3108c50755b"; 
var publicKey = "a626b5aa437ad6f953dd6a8460cf1096"; 

var hash = CryptoJS.MD5(ts + privateKey + publicKey).toString();
console.log(hash);
//6d5b79bca2f0244f4c207aef2cd8cd30