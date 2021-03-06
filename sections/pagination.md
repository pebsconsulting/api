# Pagination

Requests that return multiple items will be paginated to 25 results by default. You can specify further pages with the `page` parameter.

http://api.official.fm/playlists/search?api_version=2&q=mac+miller&page=2

Here is an example of a paginated response:

```javascript
{
  "page": 2,
  "total_entries": 40,
  "total_pages": 2,
  "playlists": [
  {
    "playlist": {
      "name": "Macadelic",
      "url": "http://api.official.fm/playlists/1rp7",
      "page": "http://official.fm/playlists/1rp7",
      "buy_url": "http://official.fm/purchases/new?playlist_id=1rp7",
      "rough_view_count": null,
      "rough_play_count": null,
      "rough_download_count": null,
      "tracks_count": 15,
    "project": {
      "name": "Mac Miller",
      "url": "http://api.official.fm/projects/f8w6"
    }
  }
  ...
}
```