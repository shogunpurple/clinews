# clinews :earth_africa: :newspaper: :computer:
[![npm](https://img.shields.io/npm/dt/clinews.svg)](https://www.npmjs.com/package/clinews)
[![npm](https://img.shields.io/npm/v/clinews.svg)](https://www.npmjs.com/package/clinews)
[![license](https://img.shields.io/github/license/mmckeaveney/clinews.svg)](https://github.com/mmckeaveney/clinews/blob/master/LICENSE)

A CLI for reading the news which supports over 70 sources. Get all the latest headlines from around the world without leaving your terminal. Powered by [NewsAPI.org](https://newsapi.org/).

clinews allows you to:

- Fetch all the latest stories from a particular news source
- List all possible news sources the API provides
- Search across all the sources for a particular word or phrase in the title.

## Installation
Note: You must be on node version **7.6.0** or later to use clinews.

**npm** 
```
npm i -g clinews
```

**yarn** 
```
yarn global add clinews
```

## Usage

### Fetch stories from a source
Fetch all the latest news stories from bbc-news: 
```
news fetch bbc-news
```

other examples...
```
news fetch techcrunch
news fetch hacker-news
```

### List all news sources
Show all the sources you can get news from. Use the ```Fetch Id``` field with the ```fetch``` command to get news for that source.
```
news sources
```

### Search for news stories across all sources matching search criteria

You can search across all 70+ news sources to find stories with a title matching your criteria. For example, to find all news stories with titles containing the words "Donald Trump" you can execute the following. Note that searches are also case insensitive. The 2 commands below are equivalent.

```
news search "Donald Trump"
```
or
```
news search "donald trump"
```

## Options

clinews supports some extra flags as well. See below:
```
-V, --version              output the version number
-l, --limit <limit>        limit the amount of news stories you want to see.
-s, --sort <sort>          sort to apply to the news stories, Choices include top, latest or popular.
-c, --category <category>  category of sources you want to see. Choices include: business, entertainment, gaming, general, music, politics, science-and-nature, sport, technology.
-h, --help                 output usage information
```

You can run ```news --help``` to get this information at any time.





