# Next-js-fullcourse

https://www.youtube.com/watch?v=KjY94sAKLlw

https://www.youtube.com/watch?v=VE8BkImUciY



Nextjs:
-------

Next.js is a backend framework which is based on React.

Everything we can do in React we can also do in Next.js – with some additional features like routing, API calls, authentication, and more. We don’t have these features in React. Instead, we have to install some external libraries and dependencies – like React Router for routing in a single page React app, for example.

But in Next.js, things are different. We don’t have to rely on external libraries to get these kinds of things done. They come built into the package when we create a Next.js app.

This is the main reason why a Next.js app is different from a traditional React app.

Next js Re-rendering SSR and CSR:
---------------------------------

How does CSR Work?

When you visite your website the server receives the request and sends an empty HTML file and a bunch of bundled Javascript , and your browser processes those bundles and renders the final HTMl file  so the initial page lead speed of the application can be slow because of this process, and since the page is built on the user is browser, search engines cannot index
website properly but on the server side rendering, when you visite the website the server receives the request and renders the HTML page and sends 
that to your browser, so if we a have an old computer or phone it is really good because your browser doesnt have to render everything from scratch, so it shows the initial page faster but since everything happens on server side you wont be able to intract with the user, if you want to create an event you have to create a client side component, so if you have a highly
intractive website it might be really annoying basically chossing SSR and CSR depends on your project.


That is why next-js is greate because you can combine server side and client side components and build a complete application 

NextJs images
--------------

To add an image we are not going to be useing image HTML <img /> , it will display a warning  we will use <Image />


NextJs Fetching 
---------------


Fetching Data Where It's Needed
If you need to use the same data (e.g. current user) in multiple components in a tree, you do not have to fetch data globally, nor forward props between components. Instead, you can use fetch or React cache in the component that needs the data without worrying about the performance implications of making multiple requests for the same data.

Promise (then() and catch()) ---> (Async() and await)
------------------------------------------------------

What is javascript promises ? why we need them ? How to use the special then() and catch()methods and then how to convert the same code to using async() and await()


The promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value



use the fetch API built into the browser in order to make asynchronous request to different network ressources by using GET, POST , PUT or whatever it is that you want to use 


Fetch is promise based which means that we can use async await or we can use .then() or .catch()


--> you want to do more tha Get data from the server (you want to post , update and delete data so in order to do that you are going to need to use the options section of the fetch method   )

fetch("https://reqres.in/api/users", {
    method: POST (choose the HTTP method),
    (we need to pass the data for that user and that is going to go inside of the body  )

    --> To save our user we should (send it JSON) so add JSON.stringify and we should add headers
    headers : {
        'Content-Type' : 'application/json'
    }
    body: JSON.stringify({
        name : 'User 1'
    })
}).then(res => {
    return res.JSON();
})
.then(data => console.log(data))
.catch(error => console.log(Error'))

---> so we have to convert javaScript data to JSON string



<img width="1303" alt="Screen Shot 2023-08-14 at 1 42 55 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/32cba704-3114-4825-b2bf-216d526e17d1">


<img width="1303" alt="Screen Shot 2023-08-14 at 1 43 03 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/9f73680e-a602-4ad2-8837-bee05fd2ceb0">


<img width="1303" alt="Screen Shot 2023-08-14 at 1 43 14 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/ec573121-93fd-4e7c-a3d3-9fcbc2c50b9b">

<img width="2400" alt="Screen Shot 2023-08-16 at 8 12 56 AM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/95075613-ef5b-4241-a0a6-7e0394f970e1">

<img width="2400" alt="Screen Shot 2023-08-16 at 8 13 07 AM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/1a4445ff-f9d2-4092-b3cc-28c03803468d">


<img width="2400" alt="Screen Shot 2023-08-16 at 8 13 17 AM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/a1ed816b-cc3c-4aa0-b2ab-4604e088e525">

<img width="2349" alt="Screen Shot 2023-08-16 at 1 56 28 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/dd40940f-a911-4d05-98cf-3aca04ce89ac">






<img width="2349" alt="Screen Shot 2023-08-16 at 1 56 00 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/351d7158-70f7-4617-be34-46e400f61a4b">

<img width="2349" alt="Screen Shot 2023-08-16 at 1 56 14 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/4ce8fdb7-3ab9-4809-84ab-6937fbd89f14">






<img width="1235" alt="Screen Shot 2023-08-14 at 4 02 30 PM" src="https://github.com/SouchenOu/Next-js-fullcourse/assets/87101785/10d64d50-b6e5-4897-9f60-d73cef1d39eb">



