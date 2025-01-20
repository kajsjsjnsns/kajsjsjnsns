const axios = require('axios');

const uid = 'Randomuid support';
const region = 'rn';
const key = 'Pranto69';
const url = `https://garena420ffapi.vercel.app/profile_info?uid=${uid}&region=${region}&key=${key}`;

axios.get(url)
  .then(response => {
    if (response.status === 200) {
      console.log('99+ visit sent successfully');
    } else {
      console.log('Something went wrong');
    }
  })
  .catch(error => {
    console.error('Error:', error.message);
  });
