# Rails API

```bash
rails new my_albums --api --skip-action-cable --skip-sprockets
cd my_albums
bundle
rails g scaffold Album title:string released:string
rake db:migrate
```

Insert some data:

```bash
curl -X POST localhost:3000/albums -H "Content-Type: application/json" \
  --data '{"title":"Houses Of The Holy","released":"March 28, 1973"}'
```


## More examples

* [JSON API with Rails 5](https://www.youtube.com/watch?v=EpzIhQBXUQk)
