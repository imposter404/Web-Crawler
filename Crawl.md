# Web Crawl

# python
need libraries
- Request 

>``` python
> import request
> resp =request.get(URL)
> print("status ": resp.status_code);
> print("response")
> print(resp.text)
>```




what i need to do ?
1. first i need the website to scrap here we are using "know your meme"
2.  i need to scrap all the images in the page with scraper
  > [!NOTE] 
  > only scrap the images with secific dimention 
> [!WARNING] 
  > DONT SCRAP IMG THUMBNAILS
3. i need to get all the links ine that wab page 
 > [!WARNING] 
 > filter out all the social media linksonly accept "know your meme" links
4. save the list in a array 
5. go forward to scrap the next link
6. continue `step 1`. 


> [!WARNING]
> while scraping the images always save the img with its url in a csv or json format 

> [!WARNING] 
> only use `JSON` OR `CSV` and nothing else

but why save th links ?
- it will be used later to find the origin of the meme and get its description of the meme
- it will be used to get the related meme accoding to the meme we found


but how to scrap web?
# JS
in JS ?
why dont i use js ?
- VANILA JS is unable to fetch the URLs cause Chrome V8 engine blocks CORS request 

How to solve it ?
- we need to use a server `NODE JS`;
- we need 3rd paty libraries to make request 
- need 
  - `Axios` for https request
  - `Cheeroi` for pursuing and manipulating HTML
  - `Puppeteer` for scraping JS heavy website using headless browser
  - `node fetch` a light weight HTTP request 
  - `request-promise` a promisebased http request library

> [!NOTE] 
> source= "GFG"

if i need i can used fully 3rd party library
`ScraperJS` available on *GITHUB*



# OR 
just use 

# PYTHON
image scrap

>``` python
> import request 
> img_url="our url" #pointing to our img and not the webpage 
> output_filename="just_a_name.png"
> response=request.get(image_url)
> if response.status_code==200
> with open(output_filename,"wb") as file:
> file.write(response.content)
> print("donloaded success as{output_filename}")
> else:
> print("failed")
>```

this will do the work i guess :)

> [!NOTE] 
> source= "GFG"

# Buuuuuuuutttttt
how can we prevent infinity loop ?
we can use `DFS` at depth limit or 
`BFS`
here `BFS` makes more sense cause it will give us the dank meme we are searching for ... yeet :)


# Frontend 

## flow chart
1. user uploads pic
2. js handles the pic and send it to Python (by Django Framework or JS->PHP->OS->Python)
3. python will do the Deep learnig with the data set of pics we alreay scraped 
4. it will give the best match pic with its link 
5. and the hatefull meter 
6. all the data are send from Python->JS->HTML
7. JS will handle the data and fetch the data from th url ("here know your meme or given link)
8. JS will handle the the data handeling and visualization 
9. complete :) 
10.





