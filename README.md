# MyProjects2
Ссылка на работу в Codeopen:
https://codepen.io/JuliaGrey/pen/yyBgzBJ
Детали:
HTML code:
<head>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.9.2/html2pdf.bundle.min.js"></script>
</head>
    <div class="main" id="main">
      <div class="head">
        <img class="Avatar" src="https://i.pinimg.com/736x/31/81/62/318162c9ca44fcf87857bc48dc9da447.jpg" />
        <div class="nameBox">
          <div class="greetingPhrase">Привет! Я</div>
          <div class="yourInfo">
            <div class="name" onclick="changetext(this)">Исаевич Юлия</div>
            <div class="role" onclick="changetext(this)">Студентка СибГУТИ</div>
          </div>
        </div>
        <div class="languagesBox">
          <div class="title">Языки:</div>
          <div class="english" onclick="changeLanguage(this)">
            Английский
            <img
              class="engflag" id= "flag"
              src="https://www.a1flags.com.au/images/Catalogue/Flag/uk---.svg"
              alt="Флаг Англии"
            />
          </div>
          <div class="russian" onclick="changeLanguage(this)">
            Русский
            <img
              class="rusflag" id="flag"
              src="https://sc24-surgut.gosuslugi.ru/netcat_files/userfiles/Ofitsal_no/Flag_Rossii_1_.jpg"
              alt="Флаг России"
            />
          </div>
          <div class="german" onclick="changeLanguage(this)">
            Немецкий
            <img
              class="gerflag" id="flag"
              src="https://www.labelocean.de/ae/Germany/Flaggen/ES-FL-DEU.jpg"
              alt="Флаг Германии"
            />
          </div>
        </div>
      </div>
      <div class="body">
        <div class="expBox">
          <div class="title">Опыт</div>
          <div class="exp" onclick="changetext(this)">
            Закончила 1 курс обучения на направлении Программное обеспечение мобильных систем, получила оценку "отлично" по дисциплинам "Технологии программирования", "САОД", "Физика" и "Дискретная математика", также я всегда проявляла инициативу в изучении чего-то нового и училась работать в команде, завела много полезных знакомств и побывала на нескольких митапах от Т-Банка.
          </div>
        </div>
        <div class="toolsBox">
          <div class="title">Навыки</div>
          <div class="tools">
            <ul>
              <li onclick="changeLi(this)"><span>Photoshop</span></li>
              <li onclick="changeLi(this)"><span>C++</span></li>
              <li onclick="changeLi(this)"><span>C</span></li>
              <li onclick="changeLi(this)"><span>GitHub</span></li>
              <li onclick="changeLi(this)"><span>Figma</span></li>
              <li onclick="changeLi(this)"><span>HTML+CSS+JS</span></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="foot">
        <div class="educationBox">
          <div class="title">Образование</div>
          <div class="schoolBox">
            <div class="school" onclick="changetext(this)">МБОУ Лицей №3 Среднее общее</div>
          </div>
          <div class="schoolBox">
            <div class="school" onclick="changetext(this)">СибГУТИ ИВТ Программное обеспечение мобильных систем 2 курс</div>
          </div>
        </div>
        <div class="box">
          <div class="interestsBox">
            <div class="title">Интересы</div>
            <ul>
              <li onclick="changeLi(this)"><span>Программирование</span></li>
              <li onclick="changeLi(this)"><span>Моделирование</span></li>
              <li onclick="changeLi(this)"><span>Изучение ин. языков</span></li>
              <li onclick="changeLi(this)"><span>Игра на музыкальных инструментах, вокал</span></li>
            </ul>
          </div>
          <div class="contactBox">
            <div class="title">Контакты</div>
            <div class="contactText">Номер телефона:</div>
            <div class="phoneNumber" onclick="changetext(this)">+7(913)760-97-88</div>
            <div class="contactText">Почта:</div>
            <div class="email" onclick="changetext(this)">juliaei2005@mail.ru</div>
          </div>
        </div>
      </div>
      <div class="PDFbutton">
        <button onclick="captureImage()">Скачать</button>
      </div>
    </div>

    CSS code:
    * {
  box-sizing: border-box;
}

.main{
    display: flex;
    flex-direction: column;
    position: absolute;
    width: 555px; 
    height: 812px; 
    top: 15px;
    left: 20px;
    gap: 20px; 
  border: 1px solid #000; /* Для наглядности */
}

.head {
  gap: 20px;
  display: flex;
}

.Avatar {
  width: 124px;
  height: 124px;
  border-radius: 12px;
}

.nameBox {
  background-color: rgb(215, 215, 215);
  width: 124px;
  height: 124px;
  padding: 12px;
  border-radius: 12px;
}

.greetingPhrase {
  width: 100px;
  height: 24px;
  font-family: Poppins;
  font-size: 15px;
  color: rgb(0, 0, 0);
  text-align: center;
  font-weight: bold;
}

.name {
  width: 100px;
  height: 30px;
  font-family: Poppins;
  font-size: 13px;
  text-align: center;
}

.role {
  width: 100px;
  height: 24px;
  font-family: Poppins;
  font-size: 11px;
  text-align: center;
}

.languagesBox {
  background-color: rgb(215, 215, 215);
  width: 170px;
  height: 124px;
  padding: 12px;
  border-radius: 12px;
}

.title {
  height: 21px;
  font-family: Poppins;
  font-size: 16px;
  font-weight: bold;
  text-align: center;
}

.english {
  height: 20px;
  font-family: Poppins;
  font-size: 15px;
  display: flex;
}

.engflag {
  width: 24px;
  height: 14px;
  border-radius: 12px;
}

.russian {
  height: 20px;
  font-family: Poppins;
  font-size: 15px;
  display: flex;
}

.rusflag {
  width: 24px;
  height: 14px;
  border-radius: 12px;
}

.german {
  height: 20px;
  font-family: Poppins;
  font-size: 15px;
  display: flex;
}

.gerflag {
  width: 24px;
  height: 14px;
  border-radius: 12px;
}

.body {
  display: flex;
  gap: 16px;
}
.expBox {
  background-color: rgb(215, 215, 215);
  width: 300px;
  height: 300px;
  padding: 12px;
  border-radius: 12px;
}

.exp {
  height: 250px;
  font-family: Poppins;
  font-size: 15px;
  display: flex;
  text-align: center;
}
.toolsBox {
  background-color: rgb(215, 215, 215);
  width: 145px;
  height: 180px;
  border-radius: 12px;
}

.tools {
  height: 20px;
  font-family: Poppins;
  font-size: 15px;
  display: flex;
}
.foot {
  gap: 20px;
  display: flex;
}
.educationBox {
  background-color: rgb(215, 215, 215);
  width: 220px;
  height: 300px;
  padding: 12px;
  border-radius: 12px;
}
.interestsBox {
  background-color: rgb(215, 215, 215);
  width: 220px;
  height: 170px;
  padding: 12px;
  border-radius: 12px;
  margin-bottom: 12px;
}
.schoolBox {
  background-color: rgb(40, 217, 121);
  width: 195px;
  height: 100px;
  padding: 12px;
  margin-bottom: 12px;
  border-radius: 12px;
}
.contactBox {
  background-color: rgb(215, 215, 215);
  width: 220px;
  height: 120px;
  padding: 12px;
  border-radius: 12px;
}
.contactText {
  font-size: 14px;
  font-family: Poppins;
  font-weight: bold;
  text-align: center;
}
.PDFbutton {
  margin-left: auto;
  margin-right: auto;
}
.button {
  background-color: rgb(229, 81, 81);
  width: 220px;
  height: 60px;
  border-radius: 12px;
}
.PDFtext {
  font-size: 20px;
  font-family: Poppins;
  font-weight: bold;
  height: 60px;
  line-height: 60px;
  text-align: center;
}
.saveButton{
    font-weight: bold;
    width: 200px;
    margin-left: auto;
    margin-right: auto;
}

JS code:

function changetext(div) {
    var input = document.createElement('input');
    input.type = 'text';
    input.value = div.innerText;
    
    input.onblur = function() {
        div.innerText = input.value;
        div.style.display = 'block';
        input.remove();
    };

    div.style.display = 'none';
    div.parentNode.insertBefore(input, div);
    input.focus();
}

function changeLanguage(div) {
    var flag = div.querySelector('img');
    var input = document.createElement('input');
    input.type = 'text';
    input.value = div.childNodes[0].nodeValue.trim();

    input.onblur = function() {
        div.childNodes[0].nodeValue = input.value;

        if (input.value.toLowerCase() == 'английский') {
            flag.src = 'https://www.a1flags.com.au/images/Catalogue/Flag/uk---.svg';
        } else if(input.value.toLowerCase() == 'русский') {
            flag.src = 'https://sc24-surgut.gosuslugi.ru/netcat_files/userfiles/Ofitsal_no/Flag_Rossii_1_.jpg';
        } else if(input.value.toLowerCase() == 'немецкий') {
            flag.src = 'https://www.labelocean.de/ae/Germany/Flaggen/ES-FL-DEU.jpg';
        }
        else {
            flag.src = 'https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Noun-question-By_Adrien_Coquet%2C_FR.svg/640px-Noun-question-By_Adrien_Coquet%2C_FR.svg.png';
        }

        div.style.display = 'block';
        input.remove();
    };

    div.style.display = 'none';
    div.parentNode.insertBefore(input, div); 
    input.focus();
}

function changeLi(li){
    var span = li.querySelector('span');
    var input = document.createElement('input');
    input.type = 'text';
    input.value = span.innerText;
    
    input.onblur = function() {
        span.innerText = input.value;
        li.style.display = 'block';
        input.remove();
    };

    li.style.display = 'none';
    li.parentNode.insertBefore(input, li);
    input.focus();
}
     

       function captureImage() {
            const element = document.getElementById('main');
            html2canvas(element, {
                useCORS: true,
                scale: 2
            }).then((canvas) => {
                const image = canvas.toDataURL('image/png');
                const link = document.createElement('a');
                link.href = image;
                link.download = 'screenshot.png';
                link.click();
            });
        }
