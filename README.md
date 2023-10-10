# BE Foodmarket

## Table of Contents

1. [Description](#description)
2. [Feature](#feature)
3. [Feature Specific Information](#feature-specific-information)
4. [Database Design (ERD)](#database-design-erd)
5. [API Information](#api-information)

## Description
- This repository was created to learn how to create restful api using laravel 10.

## Feature 
1.  Authentication (Login, Register, Logout)
2.  Food List (list of foods with descriptions)
3.  Transaction List (list of transactions with their payment status)
4.  Payment gateway using midtrans
5.  Content Management System

## Feature Specific Information
1.  Authentication using a ```sanctum package``` from laravel
2.  Upload image using laravel storage
3.  Filter foods based on various criteria such as price range and rate range
4.  Filter transactions based on various criteria such as food_id and payment status

## Database Design (ERD)
<p align="center">
  <img src="https://github.com/yohanes59/foodmarket-backend/assets/80000614/649e0c5f-93e6-43cc-94d3-625b84b2d019" width="90%" height="90%">
</p>


## API Information
Noted: because here I use the default localhost link from Laravel ``` (http://127.0.0.1:8000) ```, so you can **change the link to be your localhost link**
  <table style="width: 100%; margin:0 10px; text-align: left;">
    <tr>
      <th>*</th>
      <th>API</th>
      <th>Method</th>
      <th>Request</th>
      <th>Information</th>
    </tr>
    <tr>
      <td>1</td>
      <td>http://127.0.0.1:8000/api/login</td>
      <td>POST</td>
      <td>email, password</td>
      <td>User login endpoint. Send user's email and password to authenticate and receive a token for access.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>http://127.0.0.1:8000/api/register</td>
      <td>POST</td>
      <td>name, email, password, password confirmation, address, house number, phone number and city</td>
      <td>User registration endpoint. Register a new user by providing name, email, password, password confirmation, address, house number, phone number and city.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>http://127.0.0.1:8000/api/user</td>
      <td>POST</td>
      <td>name, email, password, password confirmation, address, house number, phone number and city</td>
      <td>Update user profile data.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>http://127.0.0.1:8000/api/user</td>
      <td>GET</td>
      <td>-</td>
      <td>Get user data.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>http://127.0.0.1:8000/api/user/photo</td>
      <td>POST</td>
      <td>profile photo</td>
      <td>Update user photo.</td>
    </tr>
    <tr>
      <td>6</td>
      <td>http://127.0.0.1:8000/api/logout</td>
      <td>POST</td>
      <td>-</td>
      <td>Logout user.</td>
    </tr>
    <tr>
      <td>7</td>
      <td>http://127.0.0.1:8000/api/food</td>
      <td>GET</td>
      <td>-</td>
      <td>Show list of foods data.</td>
    </tr>
    <tr>
      <td>8</td>
      <td>http://127.0.0.1:8000/api/transaction</td>
      <td>GET</td>
      <td>-</td>
      <td>Show list of transactions data.</td>
    </tr>
    <tr>
      <td>8</td>
      <td>http://127.0.0.1:8000/api/checkout</td>
      <td>POST</td>
      <td>-</td>
      <td>Checkout the food you want to buy.</td>
    </tr>
</table>
