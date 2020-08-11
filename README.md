# simple node project
this is a learning note for me about how to create a simplest website with Node, Express, and ejs. 

- - -  
### Structure:  
>bin/www  
set up port, create server, set up event listener, view engine setup  
*ejs*  
`app.set('views', path.join(__dirname, 'views'));
app.set('view engine', 'ejs');`
*html*  
`app.use(express.static(path.join(__dirname, 'public')));`

>>app.js  
connect everything, error handler, set up routes

>>>routes/indes.js  
`router.get('/', function(req, res, next) {
  res.render('index', { title: 'Express' });
});`  
- - -  
### *Some References:*

'Building a Website with Node.js Node.js' on [LinkedIn Learning] <https://www.linkedin.com/learning/building-a-website-with-node-js-and-express-js-3)>.  
七天学会NodeJS <https://nqdeng.github.io/7-days-nodejs/>  
一起学 Node.js <http://shouce.jb51.net/yiqixue-nodejs/index.html>  
Node + Express 完全新手教學 - 4 [套用bootstrap + code分類 ] <https://www.kdzone.net/2016/01/node-express-4-bootstrap-code.html>  
构建您的第一个 Node.js 网站(两部分) <https://www.ibm.com/developerworks/cn/web/wa-simplenode1-app/index.html> https://www.ibm.com/developerworks/cn/web/wa-simplenode2-app/index.html  


