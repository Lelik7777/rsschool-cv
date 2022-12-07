# Aleksey Kvachkov

***


![](https://avatars.githubusercontent.com/u/80705108?v=4)


***

### Junior Frontend Developer

***

## Contacts

* **Location**: Simferopol,Russia
* **Phone**: +79787257377
* **Email**: 21alex7777@gmail.com
* **Discord**: Lelik Jan#9196
* **GitHub**: [Lelik7777](https://github.com/Lelik7777)
* [LinkedIn](https://www.linkedin.com/in/alex-kvachkov-aa245a237/)
* [Telegram](https://t.me/Lelik_Jan)

***

## About me

I love to learn new things, because I think that acquiring new skills allows you to live an active life and feel in
demand both in society and in personal life. I like programming because it is constantly updated, forcing me to
constantly move forward and keeping a constant tone of life. It is also important that the salaries here are quite high.
In addition to programming I am fond of weightlifting, which allows me to switch and maintain a good physical shape.
Also I like reading books and being outdoors.

I am more of an introvert and perfectionist by nature.


***

## Skills and Proficiency:

* HTML,CSS
* Js/TypeScript
* React,Redux
* Git,GitHub
* WebStorm
* MUI
* AXIOS/REST API
* Formik,Lodash

***

## Code example:

```
import {TIME_TIMEOUT} from "./config";

const timeout = function (s) {
    return new Promise(function (_, reject) {
        setTimeout(function () {
            reject(new Error(`Request took too long! Timeout after ${s} second`));
        }, s * 1000);
    });
};
//используем эту универсальную ф-цию вместо sendJson and getJson
//если uploadData нет, то обычный get request,иначе post request
export const AJAX = async (url, uploadData = undefined) => {
    try {
        const fetchPro = uploadData
            ? fetch(url, {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(uploadData),
            })
            : fetch(url);

        let res = await Promise.race([fetchPro, timeout(TIME_TIMEOUT)]);
        const data = await res.json();

        if (!res.ok) throw new Error(`${data.message}(Status:${res.status})`);

        return data;
    } catch (e) {
        throw e;
    }
}

```

***

## Experience

* My pet projects: [CARDS](https://freiii21.github.io/friday-project/#/login)
  , [Social network](https://lelik7777.github.io/social_network_2021/#/)
  ,  [To Do List](https://lelik7777.github.io/login)
* Internship at the company **Webstap** four months in 2022

***

## Courses:

* **IT-Incubator** 2021-2022
* **UDEMY**:Jonas Schmedtmann [
  complete-javascript-course](https://github.com/Lelik7777/complete-javascript-course)

***

## Languages:

* *English*: A2
* *Russian*: Native

