# Debugging

## Locally

You can debug your instance of slack-gamebot with a built-in console.

```text
2.2.1 > Game.map(&:name)
=> ['pong', 'pool']
```

## Silence Mongoid Logger

If Mongoid logging is annoying you.

```ruby
Mongoid.logger.level = Logger::INFO
Mongo::Logger.logger.level = Logger::INFO
```

## Heroku

```text
heroku run script/console --app=...

Running `script/console` attached to terminal... up, run.7593

2.2.1 > Game.count
=> 3

2.2.1 > Game.last
=> #<Game _id: 55c8f7da276eaa0003000000, ...>
```

