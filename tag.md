##### Create 1 tag at current commit	

```bash
git tag <tag-name>
```

##### Create 1 tag at old commit

```bash
git tag -a <tag-name> <commit-hash>
```

##### Delete tag

```php
git tag -d <tag-name>
```

##### Rename tag

```bash
git tag <new-name> <old-name>
git tag -d <old-name>
```


##### Push tag to remote

```bash
git push origin <tag-name>
```

##### Pull tag

```bash
# all tags
git pull origin

# sepecify tag
git pull origin <tag-name>
```
