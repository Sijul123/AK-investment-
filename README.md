# AK-investment-
This app is very good : It is a very investment-app/
├─touch app.js─ backend/
│ express.js├── app.js
│ mkdir models├── models/
│ id  │name├ email─password─ User.js
│id │user id├amount─investment type─ Investment.js
│ mkdir routes├── routes/
│/api/auth/login│/api/auth/register├/api/auth/logout── auth.js
│/api/investments│/api/investment /:id├/api/investment/crate─/api/investment/update/:id:─/api/investment/delete/:id:investments.js
│ mkdir controllers  ├── controllers/
│login│register│logout├── authController.js
│getAllInvestments│getInvestmentById│createInvestment│updateInvestment│deleteInvestment├── investmentController.js
│mkdir config├── config/
│```
// config/db.js
const mongoose = require('mongoose');

mongoose.connect('mongodb://localhost:27017/mydatabase', {
  useNewUrlParser: true,
  useUnifiedTopology: true
});

const db = mongoose.connection;

db.on('error', (err) => {
  console.error(err);
});

db.once('open', () => {
  console.log('Database connection established');
});

module.exports = mongoose;
```│   └── db.js
│mkdir middleware├── middleware/
│   │   └── authMiddleware.js
├── frontend/
│   ├── src/
│   │   ├── App.js
│   │   ├── components/
│   │   │   ├── Login.js
│   │   │   ├── Register.js
│   │   │   ├── Dashboard.js
│   │   │   ├── InvestmentList.js
│   │   └── services/
│   │       └── authService.js
│   │       └── investmentService.js
│   ├── public/
│   │   └── index.html
│   ├── package.json
│   └── .env
├── .gitignore
├── README.md app : Invest your money and earn money thank you
