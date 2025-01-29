#translaxify

- [x] Get a sample website as an example
- [x] Detect text in foreign languages 
- [x] Convert to English
- [x] Overlay with a div with the required text 


Target website -->  [Mangadex website](https://mangadex.org/chapter/fb1b38d6-f482-41fc-ab8f-90dba822f31c/2)

Steps --> 
- [x] Get all images from the loaded page
- [x] Get the appropriate contours at which the text is located
- [x] OCR the image 
- [x] Create a server endpoint out of this thingamajig
- [x] Call this endpoint from js
- [x] now overlay divs where the text was detected in the image or maybe overwrite the image itself?
- [x] Get js to reach out to this generate
- [x] Fix the website
- [x] Fix https on backend
- [ ] Setup an email list service for the server

## Approach 1
- [ ] Integrate Login into the website and create a user page for the user to actually see what the hell is going on.

- [ ] Integrate Chatgpt for this into the server, and test the setup with the vps 
	- [ ] Get Japanese Language Conversion working 
	--> Sample comic for japanese --> 
	https://nc.tameshiyo.me/9784094066289

	Ok so openAI is fucked, ohh fuck me , fuck me, fuck openai cancelling my credits, I want my money backkkkkkk
	Son of a bitch

## Approach 2 
- [x] Reassign the deepskull.in domain to the vps to handle requests
- [x] Google cloud offers free 300 credits, use google ocr for getting the text instead of fast ocr
- [x] Google Translate to translate text to another language then ??
- [x] All in all two api calls and 
- [x] Create server endpoint for that also 
- [x] 3 major things Pdfs, EPUB, Images  --> 
	- [x] Images 
	- [x] Pdfs 
	- [x] EPUB
- [x] Setup Basic Frontend for the all the UI
- [x] Create a landing page
- [x] Create Login and Signup Endpoints
- [x] Setup translation endpoints
	- [ ] Optimized the fucking pdf endpoint create a multiprocessing threadpool and then process each page from there. Wow so modern, so mature and so demure. 

#### Do Later -->
- [ ] convert to an extension, configure it to work with other api's than google gemini 
- [ ] Implement rate limiting 
- [ ] Look at storage solutions ? 
- [ ] Make the site work on mobile
- [ ] Real time monitoring 
- [ ] Create the extension to take in an api key and call it for some page
- [ ] Send only the Bounding box ,text size and font type from the backend stitch the image on the frontend
- [ ] setup proper logging for the exceptions

User Attributes --> 

basic user model

| Attribute Name    | Type                                 |
| ----------------- | ------------------------------------ |
| Email             | String                               |
| Password          | Hash(String)                         |
| Username          | String                               |
| Plan Status       | Enum of Yes or No                    |
| Plan Start Date   | Optional Datetime                    |
| Plan End Date     | Optional Datetime same as Plan start |
| Remaining Credits | Integer                              |
|                   |                                      |


https://github.com/razorpay/razorpay-node/blob/master/examples/index.js