# JHipster generator (v5.8.2) for Angular Material

This generator for Angular Material v7 overwrite the master of the generator-jhipster (v5.8.2).

## Build

### Clone the repo
```bash
mkdir -p ~/github/contribution-jhipster-uga/
cd ~/github/contribution-jhipster-uga/
git clone git@github.com:contribution-jhipster-uga/generator-jhipster.git
```

### Build the generator
```bash
cd ~/github/contribution-jhipster-uga/generator-jhipster
git branch
git checkout angular-material
git branch

#npm set prefix ~/.npm
#PATH="$HOME/.npm/bin:$PATH"
#PATH="./node_modules/.bin:$PATH"
npm install -g
```


### Test the generation
```bash
cd ~/github/contribution-jhipster-uga/
#mv test-generator-jhipster-angular-material/node_modules ./__node_modules
rm -fr test-generator-jhipster-angular-material
mkdir test-generator-jhipster-angular-material
mv __node_modules test-generator-jhipster-angular-material/node_modules
cd test-generator-jhipster-angular-material
cp ../generator-jhipster/test/mat-app-sample.yo-rc.json .yo-rc.json
jhipster --debug
npm link generator-jhipster
jhipster --debug import-jdl ../generator-jhipster/test/mat-app-sample.jh
```

### Launch the backend
```bash
cd ~/github/contribution-jhipster-uga/test-generator-jhipster-angular-material
./mvnw
```

### Launch the Angular Material frontend
```bash
cd ~/github/contribution-jhipster-uga/test-generator-jhipster-angular-material
yarn start
```

## TODOLIST

* Refactor the generator as a blueprint
* Move to Angular v8 and JHipster v6
* Remove all Bootstrap CSS classes in elements
* Material Design good practices https://material.io/design/

### client
* admin : continue to add material buttons, inputs, ...

### entity-client
* date
* image blob
* blob
* search
* mat-paginator --> i18n
* infinite-scroll
* pager
* entity-management.component --> mat-list


## References
* https://material.angular.io/
* https://material.io/design/
* Theming with wonderful http://mcg.mbitson.com/#!?mcgpalette0=%23ea1212&themename=mcgtheme  :heart:  :heart: