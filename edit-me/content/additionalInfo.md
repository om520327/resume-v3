---
title: Personal Projects
---

- Movie Website
  • Developed a movie website using Java for the backend, connecting it to MongoDB.
  • Utilized Axios to implement POST and GET requests to interact with the database.
  • Designed the frontend of the application using React.
  • Implemented functionality to view YouTube trailers and write reviews for each movie, which were stored in MongoDB.
- Social Media Clone
  • Created a social media clone using React for the frontend and Firebase for the database.
  • Implemented features such as user account creation, login authentication, profile editing, post creation, commenting,
  liking, profile picture uploading, and adding friends.
  • Designed and implemented various pages, including home, profile, add friends, login, and register pages.
- Web Crawler
  • Created a web crawler run from terminal with a website url as a parameter.
  • Created methods for normalizing urls as well as getting urls from html.
  • Created test methods using jest to insure the programs methods worked correctly.
  • Created functionality for presenting how many hits a certain url got during the crawl.
  • Created functionality to have the data displayed in terminal in an organized way.
- Video to MP3 Converter
  • Used Micro-Service architecture to create different services for taking a video and converting it to an mp3.
  • Used Docker and Kubernetes to create/manage different containers for all the services.
  • Used Python for the code
  • User uploads a video for conversion to mp3.
  • Request hits gateway service, which stores the video on MongoDB.
  • A message is sent to a RabbitMQ queue to inform downstream services about the video for processing.
  • The Video to MP3 Converter service consumes messages from RabbitMQ.
  • It retrieves the video ID from the message and fetches the video from MongoDB.
  • The video is converted to mp3 and the resulting audio file is stored in MongoDB.
  • A new message is written to RabbitMQ to signal the completion of the conversion job.
  • The Notification Service receives this message and sends an email to the client, informing them that the new mp3 is ready
  for download.
  • The client uses a unique ID from the email, along with a JWT, to make a request to the API Gateway.
  • The API Gateway fetches the MP3 from MongoDB and serves it to the client.

All Markdown files will be rendered as rich text, so you can include features such as [links](#).
