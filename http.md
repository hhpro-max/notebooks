HTTP : Hyper Text Transfer Protocol

- HTTPS : Http Secure 

- SSL Checking : 
  
  - https://www.ssllabs.com 

- 80

- 443 

- Stage, Dev, Test , ... 
  
  - 8443
  
  - 9090
  
  - 7443
  
  - 8080
  
  - 8888
  
  - 3000

- X changed -> notif 

10 :

    stage.reza.com:8080
    

- Server ->‌سایت و خدمات دهنده 

- Client -> ما

URL Structure : 

- Browser : firefox,chrome

- https://username:password@target.tld:443/dashboard.php?email=hacker@yahoo.cm#reza
  
  - https:// -> Scheme 
  
  - target.tld -> host 
  
  - 443 -> port 
  
  - dashboard.php -> path 
  
  - email=[hacker@yahoo.cm](mailto:hacker@yahoo.cm) -> Query 
  
  - \#reza -> fragment 

    - email=hacker@yahoo.cm#reza

- https://math.com/?input=1+1  

- Curl : 
  
  ```bash
  curl https://ravinacademy.com | grep elementor
  ```

- silent mode : 
  
  ```bash
  curl https://ravinacademy.com -s | grep elementor
  ```



Client : -> Request : 

https://target.tld/?username=admin&password=admin 



https://target.com/panel 

- Request Struc : 
  
  - HTTP methods : 
    
    - GET -> Read
      
      - Show 
      
      - https://target.tld/?username=admin&password=admin --> Security Problem 
      
      - در هیسوری مرورگر دیده می شود 
    
    - POST : -> Create , login 
      
      - Send data to server 
      
      - username, password -> Credentails 
      
      - Huge file , Huge Request , Binary 
      
      - در هیسوری مرورگر دیده نمی شود 
    
    - HEAD :
      
      - without response 
    
    - PUT -> Update :
      
      - Upload malic file 
      
      - Update profile
      
      - newemail=test@test.com&name=reza&family=sh&.... 
    
    - PATCH -> Update
      
      - profile update 
      
      - برای تغییرات جزیی استفاده میشه 
      
      - درخواست تغییر ایمیل :‌
        
        - newemail=test@test.com 
    
    - DELETE
      
      - DELETE https://target.tld/profile/userid/username
    
    - OPTIONS 

    - https://google.com 

    

    POST/PUT/PATCH 

بدنه درخواست در 

body 

قرار میدهم





CURL : 

    - curl -d "input=jafar&charset=&x=" -X POST https://www.urlencoder.org -v

    - HTTP/1.1 200 OK 

            - Content-Type: application/x-www-form-urlencoded 

           - input -> jafar 

            - charset ->

            - x -> 



    - Content-Type: application/json 

        {

                "key":"value",

                "key2":"value2"

        }



- XML 







Status : وضعیت  



1XX : -> اطلاعات غیرقابل تاثیر در پردازش 



2XX : موفقعیت در درخواست

    - Register 

            - 200 

-  Return when request success



3XX : redirect 

    - /login :

            incorrect -> 3XX -> login

            correct -> 200 



4XX : Client error -> 

    /profile -> 403 

    /api/1 -> 200

/api/2 -> 403

/flkgjtsh;ldfhosobsvpxcv -> 404 





5XX : Server Error:

    - Down 

    - Username-password -> database

    - Ceredentials , token , key 

    - internl server path 

            c:\\\XXx\XX\XXX\XXX\v.asp

    - Source Code Error

    - web server disclosure information 

    - 12 int , reza string 







Request Headers:    

    - کاربرد هدر ها : 

           - احراز هویت    :

                        - Cookie 

                        - Authorization: 

            - امنیتی : 

                        - Content-Security-Policy 

            - اطلاعاتی 

                    - User-Agent

                   - Referer

           

            - reza.com 

                X-Reza-Test:1







https://www.google.com/reza.sh 

https://www.google.com:





protocol

host

port 



http://reza.com.test.com:8080/domain.php?site=google.com 





Curl: 

    - User-Agent :

                -  User-Agent: curl/7.69.1

    - curl https://rainacademy.com -v -A "Firefox"

    - curl https://rainacademy.com -v -A "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:108.0) Gecko/20100101 Firefox/108.0"



curl https://rainacademy.com -v -H "User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:108.0) Gecko/20100101 Firefox/108.0"





- Response Headers: 
  
  -    Content-Type:text/html
    
    - application/json 
    
    - plain-text 
  
  - Server :apache/2.2.4
    
    - Server: Apache/2.4.54 (Win64) OpenSSL/1.1.1p **PHP/8.1**.10
  
  - Set-Cookie
    
    - login -> username, password 
      
      - reza 
        
        - response -> set-cookie
          
          - set-cookie:PHPSESSIONID
          
          - set-cookie: JSESSIONID 
          
          - set-cookie:auth=jjklhgkhglhgolhikl
          
          - *Cloudflaire, GoDADDY, Imperva , ....*
          
          - Seo  : ## Search Engine Optimizati
          
          - account.shodan.io
            
            - این کوکی رو فقط برا این دامین بفرس 
          
          - .account.shodan.io 
            
            - *.account.shodan.io 
              
              - account.shodan.io
              
              - reza.account.shodan.io
      
      - httponly  : true -> جاوا اسکریپت به اون کیلید و مقدار دسترسی ندارد 
        
        - session=gHcBqdx5yiyT7Aps5ys7weNJY7Gs-uJG4Mtt_aEI7c1zCyKgytCwc4N1A9K9mpLbNW5dPMGbV_DzHnIH7qAno4AFlXYAAAAAAAAASvfwv2NHQdjv--4NP2F9lCiMDGNvbnRpbnVlX3VybJSMGmh0dHBzOi8vYWNjb3VudC5zaG9kYW4uaW8vlIwHX2NzcmZ0X5SMKDczZmU3ZTVhZmU5NmQ0ODVmMGJmM2U4YWQyMjRlOTcxOWJjYWI5ZTGUdYeULg; _LOCALE_=en

- Response Body : 
  
  - json 
  
  - html
  
  - text 
  
  - .... 


