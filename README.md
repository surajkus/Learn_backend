# backend_testing_01
                ---Frontend site----

App.jsx
│
├── /create_post  → CreatePost.jsx
│                     │
│                     ├── User selects image
│                     ├── User enters caption
│                     └── axios.post("/create_post")
│                              │
│                              ▼
│                         Backend stores
│                         image + caption
│                              │
│                              ▼
│                     navigate("/feed")
│
└── /feed         → Feed.jsx
                      │
                      ├── useEffect()
                      ├── axios.get("/posts")
                      ├── Backend sends all posts
                      └── map() displays image + caption
					  
					  
					  
					  
					  
					  User opens
      │
      ▼
/create_post
      │
      ▼
User selects image
      │
      ▼
User enters caption
      │
      ▼
Click Submit
      │
      ▼
handleSubmit()
      │
      ▼
FormData collects image + caption
      │
      ▼
axios.post()
      │
      ▼
Backend uploads image
      │
      ▼
Backend saves data in MongoDB
      │
      ▼
navigate("/feed")
      │
      ▼
Feed page opens
      │
      ▼
useEffect() runs
      │
      ▼
axios.get("/posts")
      │
      ▼
Backend sends all posts
      │
      ▼
setPosts()
      │
      ▼
posts.map()
      │
      ▼
Every image and caption are displayed on the screen
