# Hosting Service
### Amplify
#### Pros
- Auth and Security
- Flexible cost
- Have free tier
#### Cons

### Vercel
#### Pros
- Have free tier
#### Cons
- Fixed cost 
- No auth
- For static website

# Feasibility
### Back
we might have to create dedicated database for this project.
1. there are two type of data, a new one and the existing one. the existing one won't be a problem here, so we will discuss a new one.
2. user upload new tiff image.
3. calculate NDVI and convert to vector
4. insert into database
### Front
1. user choose data source
2. user upload or draw shape 
3. query that shape from datalake
	-	using st_contain postgis function
4. send that data back to render on frontend

# Feature
- Can choose which db/schema/table to display (can choose data source)
- default page is the latest data of a table
- must selected some table and s3 path for initial data to demo on website
- versioning


# todo
- see redshift
- write backend flow
- see amplify
- find frontend map related service for rendering map and tile on front end (probably tipg)
- browser feasibility
- 