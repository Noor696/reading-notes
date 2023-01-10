## Data Fetching

[What is SWR](https://blog.openreplay.com/beginner-s-guide-to-swr-data-fetching-in-react)

[SWR Docs](https://swr.vercel.app/)

* SWR stands for stale-while-revalidate

* SWR: Data Fetching in React ,an amazing React Hooks library that takes data fetching in React to the next level.

* SWR basically means that it performs data fetching in 3 steps:

 1. Returns cached data first (stale).
 2. Sends the fetch request (revalidate).
 3. Returns the up-to-date data.

* SWR is created by Vercel and one of its advantages is that it is a fast and lightweight package.

* **Why use SWR?**

 1. Built-in Cache + Real-Time Experience:
Using SWR’s strategy, the user sees the cached (stale) data first and requests are automatically being cached. Components will always be constantly updated with the most recent data, ensuring UI will always be fast and reactive.

 2. Auto Revalidation 
SWR ensures that the user sees the most up-to-date data. So even with multiple tabs or windows, the data is always fresh and in sync when the window/tab is refocused.

 3. Pagination
supports pagination and infinite loading of data.


Step 1: Install package ```npm install swr```

Step 2: Import useSWR ```import useSWR from 'swr'```

Step 3: Write a fetcher function ```const fetcher = url => axios.get(url).then(res => res.data)```

Step 4: Fetch Data ```const fetcher = (...args) => fetch(...args).then(res => res.json())```

Step 5: Display Data

