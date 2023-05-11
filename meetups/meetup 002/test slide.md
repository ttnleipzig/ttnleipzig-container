👀---

title: GitHub Copilot
description: Einfluss von KIs auf die Gegenwart und Zukunft der Software-Entwicklung.
tags: slide,programming
robots: noindex, nofollow
type: slide

slideOptions:
  theme: black
  transition: 'fade'

  
  
---

<style>
    li, p {
        text-align: left;
    }
    /* .slides {
        background: #0005;
        backdrop-filter: blur(6px);
        border-radius: 3rem;
    } */
    .reveal section img {
        border: 0;
    }
</style>

# React Native

## Unit Testing

---

## Things to learn

1. Linting
2. Unit Tests
2. Snapshot Tests
4. Mocks
5. Continuos Integration

---

### Linting

```json
yarn lint
yarn lint:check
yarn lint:fix
```


---

### Testing

1. Unit Tests
2. Snapshot Tests

----

#### Unit Tests

```json
yarn test
yarn test:watch
```

----

#### Snapshot Tests

```diff
FAIL  tests/src/ui/atoms/Spinner.test.tsx (16.618 s)
● <Spinner isActive={true} /> › renders correctly
    expect(received).toMatchSnapshot()

- Snapshot  - 0
+ Received  + 3

+   <Text>
+     Dirk
+   </Text>
 › 1 snapshot failed.
```

```json
yarn test:update
```



