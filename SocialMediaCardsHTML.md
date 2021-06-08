### Background
This will help you create a simple card for Twitter - this will also work for WhatsApp and other social media platforms.

![image](https://user-images.githubusercontent.com/35234925/121270659-1d753b00-c890-11eb-8dd5-31bfe6ce10f1.png)

### Code
Place the following code inside the `<head>` element.

```html
<link rel="canonical" href="{link}" />
<meta property="og:url" content="{link}" />

<meta property="og:site_name" content="{name}" />
<meta property="og:title" content="{name}" />

<meta name="twitter:card" content="summary" />
<meta name="twitter:site" content="{@twitter_handle}" />
<meta name="twitter:creator" content="{@twitter_handle}" />

<meta property="description" content="{description}" />
<meta property="og:description" content="{description}" />

<meta property="og:image" content="{icon}"/>
<meta property="og:image:secure_url" content="{icon}"/>
```

### Dynamic attributes 

Replace `{name}` with the page name

![image](https://user-images.githubusercontent.com/35234925/121270313-75f80880-c88f-11eb-86d6-07e8c8c77160.png)

Replace `{description}` with the short description you want to include for this page

![image](https://user-images.githubusercontent.com/35234925/121270379-9aec7b80-c88f-11eb-9593-4222f08330ac.png)

Replace `{link}` with the link to the page/site

![image](https://user-images.githubusercontent.com/35234925/121270405-a9d32e00-c88f-11eb-811b-3044d00bfadc.png)

Replace `{icon}` with a link to the icon you would like to display (I recommend 256x256)

![image](https://user-images.githubusercontent.com/35234925/121270462-ca02ed00-c88f-11eb-8b09-80e5e6784991.png)

You can also replace `{@twitter_handle}` with the Twitter handle to the site creator and/or author of said page.

If you don't want this, just remove those two lines.
