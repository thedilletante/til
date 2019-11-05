# Hot code reload

Found here: https://dev.to/kojikanao/hot-reload-for-nodejs-with-typescript-cel

```bash
> npm install nodemon
> echo > nodemon.js < HEREDOC
{
  "watch": ["."], // directory to watch
  "ext": "js", // extentions to filter
  "exec": "node index.js" // what to execute when change was detected
}
HEREDOC
> nodemon
