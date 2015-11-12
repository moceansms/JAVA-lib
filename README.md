JAVA sample code for integration with MoceanSMS API Server.

With MoceanSMS REST API you can send SMS message, query account balance and pricing info.

Read more over at dev.moceansms.com/restapi

Examples
--------------
import moceanSMS.moceanSMS;

1) Send SMS

    moceanSMS moceansms = new moceanSMS("api_key","api_secret");
    String rest_response = moceansms.sendSMS("Mocean", "60123456789", "Hello");
    System.out.println(rest_response);


2) Query account balance

    moceanSMS moceansms = new moceanSMS("api_key","api_secret");
    String rest_response = moceansms.accountBalance();
    System.out.println(rest_response);


3) Query account pricing

    moceanSMS moceansms = new moceanSMS("api_key","api_secret");
    String rest_response = moceansms.accountPricing("502","16");
    System.out.println(rest_response);


4) Query message status

    moceanSMS moceansms = new moceanSMS("api_key","api_secret");
    String rest_response = moceansms.messageStatus("mocean123");
    System.out.println(rest_response);
