# Android build GitHub Action

A GitHub Action for building Android projects.

<img width="300" alt="image" src="https://user-images.githubusercontent.com/3036347/51519854-c7bca700-1e2a-11e9-8c14-857ce0a9af93.png">

### Usage

```
action "Build" {
  uses = "vgaidarji/android-github-actions/build@v1.0.0"
  args = "./gradlew assembleDebug"
}
```

- `uses` specifies which action to use
- `args` contains a command to be executed inside `build` action.
See [entrypoint.sh](./entrypoint.sh) and action [Dockerfile](./Dockerfile) for implementation details.
- `secrets` are optional and should be used if your build command relies on some environment variables.

License
-------

    Copyright 2019 Veaceslav Gaidarji

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
