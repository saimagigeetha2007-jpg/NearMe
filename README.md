# Ex04 Places Around Me
## Date: 

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
html
```
1.map.html
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MAP</title>

    <style>
        h1 {
            text-align: center;
            color: rgb(39, 75, 231);
            margin-top: 20px;
        }

        img {
            display: block;
            margin-left: auto;
            margin-right: auto;
            /* width: 600px;
            height: 300px; */
            border-radius: 10px;
            margin-top: 15px;
        }

        p {
            text-align: justify;
            line-height: 25px;
            padding: 25px;
            font-size: 17px;
        }

    </style>
</head>

<body>


    <img src="{% static 'chennaiMap.png' %}" alt="SEC" usemap="#image-map">

<map name="image-map">
    <area target="_self" alt="chennai" title="chennai" href="{% url 'chennai' %}" coords="1123,355,1350,538" shape="rect"></area>
</map>

</body>

</html>

2.chennai.html
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SEC</title>

    <style>
        h1 {
            text-align: center;
            color: rgb(39, 75, 231);
            margin-top: 20px;
        }

        img {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 600px;
            height: 300px;
            border-radius: 10px;
            margin-top: 15px;
        }

        p {
            text-align: justify;
            line-height: 25px;
            padding: 25px;
            font-size: 17px;
        }

        body {
            background-color: rgb(162, 225, 248);
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
        }
    </style>
</head>

<body>

    <h1>Chennai</h1>

    <img src="{% static 'CHENNAI.jpg' %}" alt="Chennai">

    <p>
        Chennai, the capital city of Tamil Nadu, stands as one of India’s most vibrant metropolitan regions, known for its rich cultural heritage, thriving economy, and coastal charm. As a city that beautifully blends tradition with modernity, Chennai attracts people from all over the country for education, employment, health care, and tourism. One of its most iconic features is Marina Beach, one of the longest urban beaches in the world, drawing millions of visitors each year. The city is also deeply rooted in classical arts—Bharatanatyam, Carnatic music, and traditional crafts flourish in its cultural centers and auditoriums, especially during the famous December music season. Chennai’s economy is robust, powered by IT hubs, automobile industries, healthcare institutions, and educational establishments that have positioned it as a major South Indian powerhouse. Architecturally, the city offers an impressive mix of ancient temples like Kapaleeshwarar Temple, colonial-era structures such as Fort St. George, and modern skyscrapers. Chennai is also renowned for its medical tourism, with world-class hospitals and research facilities attracting patients internationally. Its warm hospitality, safe environment, and disciplined urban culture make it a comfortable place to live. The city’s cuisine, marked by dosas, idlis, filter coffee, and seafood specialties, reflects the authentic flavors of Tamil tradition. Chennai’s transport network—metro lines, suburban trains, buses, and an international airport—ensures excellent connectivity. Despite rapid modernization, the city retains its old-world charm and cultural pride. With a harmonious blend of urban development and cultural preservation, Chennai continues to evolve into a global city while staying deeply connected to its roots.
    </p>
<a href="{% url 'entrance' %}">NEXT</a>
</body>

</html>

3.entrance.html
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Entrance</title>

    <style>
        h1 {
            text-align: center;
            color: rgb(39, 75, 231);
            margin-top: 20px;
        }

        img {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 600px;
            height: 300px;
            border-radius: 10px;
            margin-top: 15px;
        }

        p {
            text-align: justify;
            line-height: 25px;
            padding: 25px;
            font-size: 17px;
        }

        body {
            background-color: rgb(162, 225, 248);
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
        }
    </style>
</head>

<body>

    <h1>Entrance</h1>

    <img src="{% static 'SAVEETHAENTRANCE.jpeg' %}" alt="Chennai">

    <p>
        Saveetha Medical College, located in Chennai, is one of India’s most distinguished institutions for medical education, research, and healthcare training. Known for its advanced infrastructure and student-friendly campus environment, the college has gained a reputation for excellence across academic and clinical domains. Its modern laboratories, digital classrooms, simulation centers, and state-of-the-art hospital facilities allow students to gain extensive hands-on training from the earliest stages of their education. The attached Saveetha Medical College Hospital, with its large patient inflow, provides students with real-time exposure to diverse medical cases, enabling them to develop practical skills and clinical confidence. The institution is also recognized for its strong focus on research, encouraging students and faculty to publish papers, participate in conferences, and engage in innovative medical studies. Saveetha places equal emphasis on holistic development, offering opportunities for sports, cultural events, and community outreach programs that help shape socially responsible medical professionals. The college fosters an environment of mentorship, with approachable faculty members who guide students academically and emotionally, ensuring a supportive learning atmosphere. Saveetha Medical College is also known for its disciplined, well-organized curriculum, incorporating modern teaching methodologies, technology-driven learning platforms, and problem-based learning approaches. The campus, surrounded by greenery and peaceful landscapes, offers a serene environment that enhances focus and well-being. With a commitment to producing compassionate, skilled, and globally competent doctors, Saveetha Medical College continues to be a preferred destination for aspiring medical professionals from across the country.
    </p>
<a href="{% url 'sse' %}">NEXT</a>
</body>

</html>

4.sse.html
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SSE</title>

    <style>
        h1 {
            text-align: center;
            color: rgb(39, 75, 231);
            margin-top: 20px;
        }

        img {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 600px;
            height: 300px;
            border-radius: 10px;
            margin-top: 15px;
        }

        p {
            text-align: justify;
            line-height: 25px;
            padding: 25px;
            font-size: 17px;
        }

        body {
            background-color: rgb(162, 225, 248);
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
        }
    </style>
</head>

<body>

    <h1>SSE</h1>

    <img src="{% static 'sse.jpg' %}" alt="Chennai">

    <p>
        Saveetha University, also known as Saveetha Institute of Medical and Technical Sciences (SIMATS), is a prominent deemed university in Chennai that offers a wide range of educational programs across medicine, engineering, dental sciences, law, physiotherapy, nursing, and diverse allied health streams. The university is recognized for its interdisciplinary approach, encouraging students to explore a variety of academic fields and engage in collaborative learning. Saveetha University has built a reputation for innovation-driven education, supported by modern infrastructure, smart classrooms, skill development labs, and an ecosystem that promotes research and entrepreneurship. Its dental college is globally acclaimed for achieving world rankings, placing the university on the international academic map. The institution promotes a student-centric environment, offering mentorship, academic guidance, and personality development programs that prepare students for leadership roles in their respective professions. Along with academics, the campus emphasizes physical fitness, arts, and community service, ensuring holistic development. The university hosts several national and international conferences, workshops, and cultural events, giving students the opportunity to gain exposure beyond textbooks. With a strong commitment to research, Saveetha University encourages publication, innovation, and clinical studies supported by well-equipped labs and high-end technology. The campus environment is vibrant yet disciplined, offering safety, greenery, and an atmosphere conducive to focused learning. The university’s emphasis on ethics, integrity, and professional excellence makes its graduates highly respected in industries and institutions worldwide. Saveetha University’s continuous growth, academic achievements, and global collaborations showcase its mission to shape future-ready professionals equipped with knowledge, creativity, and compassion.
    </p>
<a href="{% url 'sec' %}">NEXT</a>
</body>

</html>

5.sec.html
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SEC</title>

    <style>
        h1 {
            text-align: center;
            color: rgb(39, 75, 231);
            margin-top: 20px;
        }

        img {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 600px;
            height: 300px;
            border-radius: 10px;
            margin-top: 15px;
        }

        p {
            text-align: justify;
            line-height: 25px;
            padding: 25px;
            font-size: 17px;
        }

        body {
            background-color: rgb(162, 225, 248);
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
        }
    </style>
</head>

<body>

    <h1>Saveetha Engineering College</h1>

    <img src="{% static 'SEC.jpeg' %}" alt="SEC">

    <p>
        Saveetha Engineering College, located on the outskirts of Chennai, is a premier institution dedicated to
        high-quality engineering education and technological advancement. Affiliated with Anna University, the college
        offers undergraduate and postgraduate programs across major engineering departments, including Computer Science,
        Electronics, Mechanical, Civil, Electrical, and Information Technology. Known for its modern academic framework
        and industry-oriented curriculum, Saveetha Engineering College equips students with both theoretical knowledge
        and practical skills.

        The well-maintained campus features advanced laboratories, innovation centers, libraries, workshops, and
        collaborative learning spaces that support academic excellence. The college has a strong placement record, with
        partnerships and tie-ups with leading MNCs, IT firms, manufacturing industries, and research organizations that
        offer internships, training, and job opportunities.

        Saveetha Engineering College also promotes extracurricular activities, technical clubs, hackathons, cultural
        festivals, and sports events that help students develop creativity, leadership qualities, and teamwork. Faculty
        members are experienced, approachable, and dedicated to guiding students in academics, research, and career
        planning.

        Its green and spacious campus provides a peaceful environment ideal for focused learning and personal growth. By
        combining strong academics with practical exposure and a supportive learning atmosphere, Saveetha Engineering
        College continues to shape engineers who are industry-ready, innovative, and prepared to contribute meaningfully
        to society.
    </p>

</body>

</html>
```

## OUTPUT
<img width="1034" height="549" alt="Screenshot 2025-12-26 175839" src="https://github.com/user-attachments/assets/1f652e38-f0ff-4a1f-9bb7-df153966e7e2" />
<img width="1033" height="544" alt="Screenshot 2025-12-26 175847" src="https://github.com/user-attachments/assets/d92bea57-3112-44c6-9bb1-bf3f48181ac0" />
<img width="1037" height="558" alt="Screenshot 2025-12-26 175853" src="https://github.com/user-attachments/assets/2a291a07-6893-4769-9a02-901dd2390bf2" />
<img width="1027" height="549" alt="Screenshot 2025-12-26 175900" src="https://github.com/user-attachments/assets/0e3d831b-443f-455f-867a-d5cb2c1ce785" />
<img width="1039" height="550" alt="Screenshot 2025-12-26 175905" src="https://github.com/user-attachments/assets/8de20317-3a93-4e03-88d5-1d005fb0d652" />







## RESULT
The program for implementing image maps using HTML is executed successfully.
