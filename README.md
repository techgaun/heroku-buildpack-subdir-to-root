# heroku-buildpack-subdir-to-root
> A simple heroku buildpack to move sub directory to root of project

This buildpack is supposed to be used as the first buildpack
on your workspace containing multiple projects.

### Usage

- Add `heroku-buildpack-subdir-to-root` as first buildpack

```
heroku buildpacks:add --index 1 https://github.com/techgaun/heroku-buildpack-subdir-to-root.git --app <YOUR_APP>
```

- Configure `PROJECT_RELATIVE_PATH`

```
heroku config:set PROJECT_RELATIVE_PATH=packages/adminWeb --app <YOUR_APP>
```

- Configure rest of your buildpacks

- Enjoy the working deployment

- If something does not work, feel free to create an issue
