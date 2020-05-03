# Udacity Cloud Developer Program #
## Project 2 - Image Filter ##
### Gordon Seeler ###
##### Date ####
May 3, 2020
#### Summary ####
The Image Filter is a Web API that when called with the query parameter consisting of an URL image address, will return an altered version of the image smaller, black and white, and of lesser quality. This serves the purpose of controlling the size of images which tend to be large and larger.
#### Description ####
Implement a Web API backend service using Node.js, Typescript, and Express middleware. The Filterimage API should temporarily store an altered version of the provided image address, deleting the file after it has been successfully returned to the calling client. It is an HTTP GET operation which should return useful return messages for common mistakes and problems (refer to provided **swagger.yaml**). 

The Image Filter API has been uploaded to GitHub (see below repo link). It also has been deployed to pubic cloud employing the AWS Elastic Beanstalk service (see endpoint below). A screen image showing the current health of the service has been provided in the `deployment_screenshots folder (Deployed_ElasticBeanstalk_Service.png)`.
#### GitHub Repository ####
https://github.com/linden416/image-filter.git
#### Installation ####
1. Clone the **image-filter.git** repository locally. 
2. Change to the **image-filter** directory
3. **npm run dev** start the service
4. Run requests to http://localhost:8082
5. A Postman file **Postman_Collection.postman_collection.json** has been provided
#### AWS Elastic Beanstalk Endpoint ####
http://image-filter-dev-dev.us-east-2.elasticbeanstalk.com
#### Try it ####
Open Postman and use the provided Postman collection file to run either a local or remote cloud test, or simply click the link below to the AWS Cloud Elastic Beanstalk service:
http://image-filter-dev-dev.us-east-2.elasticbeanstalk.com/filteredimage?image_url=https://s.yimg.com/ny/api/res/1.2/UteI3ISK0BEEW.zprA5TIA--/YXBwaWQ9aGlnaGxhbmRlcjt3PTY0MDtoPTcwNS4yMzQxNTk3Nzk2MTQz/https://s.yimg.com/uu/api/res/1.2/7q7QUWc3dRb3crYerZ6A8Q--~B/aD00MDA7dz0zNjM7c209MTthcHBpZD15dGFjaHlvbg--/https://media.zenfs.com/en/prnewswire.com/6d072075166c695a127c5a75002fd4ca
#### Return Codes ####
```
200 Filtered Image
400 Bad Request / Image_URL is required - When query param image_url omitted
404 Not Found / File Not Found
400 Bad Request / Invalid URL
500 Internal Server Error
```
#### References ####
[JavaScript Promises and Async/Await]
(https://itnext.io/javascript-promises-and-async-await-as-fast-as-possible-d7c8c8ff0abc)

[StackOverflow - UnhandledPromiseRejectionWarning, Express.js and Node.js]
(https://stackoverflow.com/questions/51484947/unhandledpromiserejectionwarning-express-js-and-node-js)

[Reddit - How to execute a function after http response is sent successfully]
(https://www.reddit.com/r/node/comments/4rvdi5/how_to_execute_a_function_after_http_response_is/)

[MDN Web Docs - Promise.reject()]
(https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/reject)

[StackOverflow - Unhandled rejections in Express applications]
(https://stackoverflow.com/questions/33410101/unhandled-rejections-in-express-applications)

[Promises in Express.js: APIs & Testing]
(https://medium.com/@54m/promises-in-express-js-apis-testing-dd0243163d57)

[Express 4.x API]
(https://expressjs.com/en/api.html#res)

Udacity Knowledge base
https://knowledge.udacity.com/questions/120916

bluebird module
http://bluebirdjs.com/docs/getting-started.html

jsonwebtoken module
https://www.npmjs.com/package/jsonwebtoken

How to use ‘sequelize.sync()’ without difficulties
https://medium.com/@smallbee/how-to-use-sequelize-sync-without-difficulties-4645a8d96841
