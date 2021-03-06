# Dataloop

## Requirements

Make sure you've installed Node.js (4.x or higher) and npm.

Install the dependencies.

```
npm install
```

## Run

Place the CSV files containing specific party terms into the folder `data/csv/parties`, and the CSV files containing specific topic terms into the folder `data/csv/topics`.

Place your `twitterconfig.json` file in the `config` folder.

```json
{
  "key": "your_key",
  "secret": "your_secret",
  "token": "your_token",
  "tokenSecret": "your_token_secret"
}
```

### Scrape

```
bin/scraper.py db_name collection_name
```

### Sculpt

```
bin/sculptor.sh -d db_name -c collection_name
```

Make sure `db_name` and `collection_name` correspond to the CSV filenames in the `data` folder.

### Visualize

Generate the pages and the routes.

```
bin/generate.js
```

Run the application locally.

```
npm start
```
