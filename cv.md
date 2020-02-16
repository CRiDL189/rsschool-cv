# Eduard Hovar

## Junior Developer Resume
![](https://sun9-19.userapi.com/c630425/v630425615/4e289/TzdJD8oOnh0.jpg)
Let me introduce myself.
My name is **Eduard**.
My surname is **Hovar**.
I am **twenty-four**.
---
# Contact Information:
- Phone: +375447753880
- Email: govor.eduard@mail.ru
- VK: https://vk.com/edikgovor
- Github: https://github.com/CRiDL189
- Discord: CRiDL189#6994
- Telegram: @CRiDL
-----
# Summary
> Originally, I am from Zhlobin, but now I live, study and work **in Gomel**. I am single, if it's important.
I graduated Gomel State Technical University named after Pavel Suhoi in 2018, the faculty: automatic and information systems, specialization information systems and technologies in design and manufacturing.
My hobby is photography. I like taking interesting pictures.
I am a communicative, funny and kind-hearted person. People also say that I am responsible, reliable and full of energy.
-----
# Skills
- Markup Languages: HTML, CSS;
- JavaScript basics;
- version control: Git + (Github);
- Photoshop;
- Illustrator;
- Unity;
- Visual Studio;
- 3ds Max.

# Code examples
> The code is part of a game:

    using System.Collections;
    using System.Collections.Generic;
    using UnityEngine;


    public class green : MonoBehaviour {
    float horizontal;
    Rigidbody2D rb; //Сначало подключаем ригидбади для работы с физикой

    void Start () {
        rb = GetComponent<Rigidbody2D> (); 
    }
    
    void FixedUpdate () { // Создаём переменные для хранения значения наклона 
        if (Application.platform == RuntimePlatform.Android) { // и проверим на андройде ли запущена игра. Если да,
            horizontal = Input.acceleration.x; //  то узнаём значение наклона телефона по иси х
        } else {
            horizontal = Input.GetAxis ("Horizontal"); // а если нет, то устанавливаем кнопки на пк.
        } //  т.е. если -1 если влево, 0 если без изменений и 1 если вправо была ось изменена
        rb.velocity = new Vector2 (Input.GetAxis ("Horizontal") * 10f, rb.velocity.y); // а потом разгоняем нашеего персонажа, 
    } // указывая уже известные нам выше направления оси и указываем скорости, а ось Y мы не трогаем 

    void OnCollisionEnter2D(Collision2D other){ // 2) вводим метод онколижен, чтобы работать с соприкосновениями объектов
        if (other.gameObject.tag == "Platform") { // т.е. если герой, касается объекта именно с тегом Platform, 
            rb.velocity = Vector2.zero; // то мы скидываем скорость прыжка,чтобы герой не разгонялся при каждом прыжке,
            rb.AddForce (transform.up * 20, ForceMode2D.Impulse); //  и задаём импульс толчка и направляем его вверх
        }
    }
    }

# Expirience
- I have no work-experience, but I have a great desire to get it.

# Education
- 2013-2018 Gomel State Technical University named after Pavel Suhoi;
- YouTube - lessons and courses: Udemy, HTML Academy, JavaScript;
- learn.javascript.

# English
- A2 pre-intremediate, but I keep learn English to this day.

# Answers and questions

**Why do you want to leave your current job (position)?**
> Well, I want to leave my job because I don't have any perspective there. I  do monotonous work and for me it is degradation, as I am an ambitious person I want growth in my career.
-----
**Why do you want to work here (at our company)?**
> I want to work at your company because you have a young and friendly team. Also, you have a very convenient office location. Your company provides its staff with career growth, flexible working hours, free English courses and as far as, I know insurance as well. And for me it is very important.
-----
**What are your strengths and weaknesses?**
> I get on well with people. I can also connect with any person, no matter how old he is. One of my strengths is an ability to cope with any situation.
I am an optimist and I always try to look at problems and difficult situations the same way... (optimistically)
In fact, I am not afraid of problems, on the contrary, they make me stronger and more experienced.
----
**What are your weaknesses?**
> Sometimes I use my time ineffectively, I get carried away, with something and forget about everything. Unfortunately, it causes problems never the less I learn from my own mistakes.
Now I always plan my day in advance, I am not shy to ask for help. I look for more effective ways of solving this or that problem. As, sometimes I am absent-minded I always write down all tasks in my diary or daily planner in order to do then on time.
-----
