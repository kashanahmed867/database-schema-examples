# Basic blog example

```groovy
model Blog {
  id: Int @id
  name: String
  viewCount: Int
  posts: Post[]
  authors: Author[]
}

model Author {
  id: Int @id
  name: String?
  authors: Blog[]
}

model Post {
  id: Int @id
  title: String
  tags: String[]
  blog: Blog
}
```
