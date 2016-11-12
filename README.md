# PayPal_flask
PayPal example use Python Flask

* [Demo](https://youtu.be/7tlbl0e_umQ)  
(影片有更多詳細的介紹)

使用Python [Flask](http://flask.pocoo.org/) 搭配 [PayPal](https://www.paypal.com/) 網路線上付款，希望這個簡單的範例可以幫助想要學習的朋友。

## 特色
* 透過 [PayPal](https://www.paypal.com/) 網路線上付款 。
* 更多的文件可以參考 [PayPal Document](https://developer.paypal.com/docs/)

## 執行說明
請先確定電腦有安裝 [Python](https://www.python.org/)

接著使用下列指令即可運行
``` 
python app.py
```

請去 [PayPal](https://www.paypal.com/) 註冊一組帳號，註冊完畢之後，

請到 [HERE](https://developer.paypal.com/developer/applications)，點選Create App，如下圖

![alt tag](http://i.imgur.com/7yMAf04.jpg)

接著將裡面的key貼到程式碼裡
![alt tag](http://i.imgur.com/fv1z8Hn.jpg)

``` 
paypal.configure({
    "mode": "sandbox",  # sandbox or live
    "client_id": "ATcNxfmVFttFZG3v6mnrjuGGL9RzZqBZeGpPUiiarEpdzXyoe1ecgKTljdnDNfuQzBsEq3yW_YpFc_2O",
    "client_secret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"})

```

P.S KEY請換自己的!!

接著你到 Sandbox -> Accounts ，你會發現有兩組帳號，這兩組就是你的測試帳號，密碼可以再自行修改。
![alt tag](http://i.imgur.com/WNvnZeI.jpg)

這兩組帳號可以從以下的網址登入
[sandbox paypal](https://www.sandbox.paypal.com/signin)

## 執行畫面

可選擇要使用 PayPal 或 Credit Card 付款的方式
![alt tag](http://i.imgur.com/WAEAI77.jpg)

可以輸入 Sale ID 以及 金額 去 Refund
![alt tag](http://i.imgur.com/S6i7YcE.jpg)

下方顯示最近的50筆交易紀錄
![alt tag](http://i.imgur.com/pZeUjU5.jpg)


## External JS
* [DataTables](https://datatables.net/)

## 其他參考
* [PayPal-Python-SDK](https://github.com/paypal/PayPal-Python-SDK)
    
## 執行環境
* Python 3.5.2

## License
MIT license
