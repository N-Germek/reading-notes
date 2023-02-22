# React Rourtes and Deployment

## Dynamic Routes

With dynamic routes, page paths are dependant on external data. Pages that begin and end with ```[]``` are static routes and then we will set a post function inside to render it. For exampe: ```[id].js.``` Next, we will export an async function ```getStaticPaths``` that will return a list of possible values for ```id``` to route to. We will need to implement ```getStaticProps``` to retrieve the proper data with the given ```id```.

The returned list is a list of objects. Each object must have ```params``` and contain an object with ```id```.

Use the ```remark``` library to render markdown then add your imports: ```import { remark } from 'remark';
import html from 'remark-html';```.
then, update the ```getPostData()``` function in the same file. update ```getStaticProps``` to use await when you call ```getPostData()```. Finally, Update post component to render ```contentHtml```using ```dangerouslySetInnerHTML```.

## Things I want to know more about

### Resources

[NextJS Dynamic Routes](https://nextjs.org/learn/basics/dynamic-routes)

[NextJs Deployment](https://nextjs.org/learn/basics/deploying-nextjs-app)

[Next.js 10 is here! Exciting new features and updates from Next.js Conf 2020](https://www.youtube.com/watch?v=JWCS5IdECVI)

### Links

- >[Advanced Software Development](README.md)
