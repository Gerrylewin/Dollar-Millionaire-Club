
const axios = require("axios");

const options = {
  method: 'GET',
  url: 'https://weatherapi-com.p.rapidapi.com/current.json',
  params: {q: '<REQUIRED>'},
  headers: {
    'X-RapidAPI-Key': 'a76b86762dmsh25a614daa47c6f3p17e274jsneb6c03453e8b',
    'X-RapidAPI-Host': 'weatherapi-com.p.rapidapi.com'
  }
};

axios.request(options).then(function (response) {
	console.log(response.data);
}).catch(function (error) {
	console.error(error);
});
