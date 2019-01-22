# Android emulator GitHub Action

A GitHub Action for running Android UI tests on Android emulator.

<img width="300" alt="image" src="https://user-images.githubusercontent.com/3036347/51520441-5120a900-1e2c-11e9-9d86-1f367ade6e7e.png">

### Usage

```
action "Run UI Tests" {
  needs = ["Build"]
  uses = "vgaidarji/android-github-actions/emulator@v1.0.0"
}
```

Under the hood `vgaidarji/android-github-actions/emulator` action runs `./gradlew connectedAndroidTest` to run UI tests.
See [ui-tests-on-emulator.sh](https://github.com/vgaidarji/docker-android/blob/master/docker-android-emulator/ui-tests-on-emulator.sh)
script content for more details.

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
