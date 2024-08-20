
# CIPHER API

The CIPHER API offers a comprehensive suite of functionalities, including web crawling, name search, image search, IP lookup, and phone number search, enabling users to efficiently retrieve relevant information across various domains.


![Logo](http://skynethub.net/CIPHER/cbanner.png)


## Features



### IP Tracking:

CIPHER can determine a person's geographic location based on their IP address. By analyzing network data and using geolocation technologies, the program can provide precise information about a person's approximate location.

### Image Search
CIPHER's image search feature allows users to search images on Querry. 

### Search by first and last name

CIPHER allows users to search for people by their first and last name. The program accesses extensive databases that contain personal information and allows users to search for specific people in a targeted manner.

### Cell Phone Tracking
CIPHER provides users with the capability to obtain detailed information about a phone number, including the country, country code, validity, local number, currency code, carrier, and other relevant data.
## API Reference

### Get Phone Information

```http
  GET /API/search/phonenumber?query={PhoneNumber}
```
##### Example:
```http
  GET /API/search/phonenumber?query=+49 015226711959
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `query` | `string` |Phone Number |




### Crawl Web for Name & Lastname

```http
  GET /API/search/name?name={name}&lastname={lastname}&count={count}
```
##### Example:
```http
  GET /API/search/name?name=John&lastname=Doe?count=5
```


| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `name`      | `string` | **Required**. First Name |
| `lastname`      | `string` | **Required**. last Name |
| `count`      | `string` | **Required**. Count of Outputs |


### Web Crawler

```http
  GET /API/search/web?query={query}&count={count}
```
##### Example:
```http
  GET /API/search/web?query=Bitcoin&count=5
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `query` | `string` |Search Query|
| `count` | `string` |Output Count|


### Web image search

```http
  GET /API/search/image?query={query}
```
##### Example:
```http
  GET /API/search/image?query=dog
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `query` | `string` |image Search Query|

### Get IP informations

```http
  GET /API/search/ip?query={ip}
```
##### Example:
```http
  GET /API/search/ip?query=51.87.210.216

```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `ip` | `string` |IP to check|






## Author

- [@Matti Krebelder](https://www.github.com/Matti-krebelder)

