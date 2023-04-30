# Chapter 1

## 프레임워크에 대한 이야기

프레임워크에 대한 내의 생각과 프레임워크 없이 개발하는 방법을 배우는 것이 왜 중요한지

### 프레임워크란?

> 무언가를 만들 수 있는 지지 구조
> 프레임워크는 코드를 호출한다. 코드는 라이브러리를 호출한다

#### 프레임워크와 라이브러리 비교

```ts
// 프레임워크
@Injectable({
  provideIn: "root",
})
export class PeopleService {
  constructor(private http: HttpClient) {}
}

// 라이브러리
export const formatDate = (date) => {
  return moment(date).format(DATE_FORMAT);
};
```

moment는 애플리케이션 코드를 어떻게 구성해야 하는지에 대해 특별한 형식을 요구하지 않는다.
