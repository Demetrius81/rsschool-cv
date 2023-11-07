#### Ryzhou Dzmitry
---

### Junior Fullstack Developer
***

# Contact information:
**Phone:** +375 44 7154428
**E-mail:** demetrius81ryzhov@gmail.com
**Telegram:** @demetrius_q
**LinkedIn** https://www.linkedin.com/in/dmitry-ryzhov-87402a229
***

**Briefly About Myself:**
I started my career as an engineer at a car factory. Throughout this time, I have encountered new technologies, successfully studied them and applied them in the process of work.

Two years ago I decided to connect my career with software development. To do this, I enrolled in .NET development courses. I used the courses as a roadmap for my learning and learned most of the material from Microsoft documentation.
At the same time, I was interested in front-end development and studied the Vue.js framework.

I like to study and learn new things. My persistence and pedantry will definitely help me become a high-level specialist.
***

**Skills and Proficiency:**
HTML5, CSS3
JavaScript, Vue.js
C#, ASP.NET, WPF
MVC, MVP, MVVM
Python
Java
SQL
Git, GitHub
VS Code, Microsoft Visual Studio,  IntelliJ Idea,  IntelliJ PyCharm, Figma
***

JavaScript code example:

```
const saveUserData = async (user, url) => {
  if (user === null || user === undefined) {
    throw new Error(`Invalid argument: userId.`);
  }

  if (url === null || url.constructor.name !== "String") {
    throw new Error(`Invalid argument: url.`);
  }

  let response = null;
  let result = null;
  let bodyString = JSON.stringify(user);

  try {
    response = await fetch(url, {
      method: "POST",
      headers: {
        "Content-Type": "application/json;charset=utf-8",
      },
      body: bodyString,
    });

    if (response.ok) {
      result = response.status;
    } else {
      throw new Error(
        `We have some problems! Look, response status is ${response.status}.`
      );
    }
  } catch (error) {
    throw new Error(error.message);
  }

  return result;
};
```

Vue.js code example:

```
const saveUserData = async (user, url) => {
  if (user === null || user === undefined) {
    throw new Error(`Invalid argument: userId.`);
  }

  if (url === null || url.constructor.name !== "String") {
    throw new Error(`Invalid argument: url.`);
  }

  let response = null;
  let result = null;
  let bodyString = JSON.stringify(user);

  try {
    response = await fetch(url, {
      method: "POST",
      headers: {
        "Content-Type": "application/json;charset=utf-8",
      },
      body: bodyString,
    });

    if (response.ok) {
      result = response.status;
    } else {
      throw new Error(
        `We have some problems! Look, response status is ${response.status}.`
      );
    }
  } catch (error) {
    throw new Error(error.message);
  }

  return result;
};
```

c# code example :

```
/// <summary>Red-black tree node class</summary>
/// <typeparam name="T">Type that implements the interface IComparable</typeparam>
internal class Node<T> where T : IComparable<T>
{    
    public T Value { get; set; }
    internal Color Color { get; set; }
    internal Node<T>? LeftChild { get; set; }
    internal Node<T>? RightChild { get; set; }

    public override string ToString()
    {
        return $$"""Node{ "value" = "{{Value}}", "color" = "{{Color}}" }""";
    }
}
```

Java code example:

```
package org.NoteBook.Controller;

import org.NoteBook.Abstractions.Entity;
import org.NoteBook.Interfaces.ILogic;
import org.NoteBook.Interfaces.IRepository;
import org.NoteBook.Models.Contact;

import java.util.List;

public class NoteBookLogic implements ILogic {
    private final IRepository repository;
    public NoteBookLogic(IRepository repository) {
        this.repository = repository;
    }

    @Override
    public int addContact(Entity contact) {
        if (contact == null) {
            return -1;
        }
        return repository.addContact(contact);
    }

    @Override
    public List<Contact> getContacts(int from, int count) {
        if (from < 0 || count <= 0) {
            return null;
        }
        return repository.getContacts(from, count);
    }

    @Override
    public Entity updateContact(Entity contact) {
        if (contact == null) {
            return null;
        }
        return repository.updateContact(contact);
    }

    @Override
    public Boolean removeContact(int id) {
        if (id < 0 ) {
            return false;
        }
        return repository.removeContact(id);
    }
}

```
***

**Courses:**

GeekBrains ASP.NET develloper (in progress)
GeekBrains Front-end develloper (in progress)
***

**Languages:**
English - A2
Russian - Native
Belorussian - Native
***