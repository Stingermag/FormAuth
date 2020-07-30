<template>
    <div class="allsections">
        <form action="">
        <div class="section">
            <h2>Данные о пользователе</h2>
            <div class="inputtext">
                <p>Фамилия <span class="required">*</span></p>
                <input class="requir" type="text" name="secname" id="" required pattern="[A-Za-zА-Яа-яЁё\s]{2,20}" title="Колесников">
            </div>
            <div class="inputtext">
                <p>Имя <span class="required">*</span></p>
                <input  class="requir" type="text" name="name" id="" required pattern="[A-Za-zА-Яа-яЁё\s]{2,20}" title="Дмитрий">
            </div>
            <div class="inputtext">
                <p>Отчество</p>
                <input type="text" name="fathername" id="" pattern="[A-Za-zА-Яа-яЁё\s]{2,20}" title="Николаевич">
            </div>
            <div class="inputtext">
                <p>Дата раждения <span class="required">*</span></p>
                <input  class="requir" type="date" name="birthday" id="" required pattern="[0-9]{2}\.[0-9]{2}\.[0-9]{4}" title="12.04.2020">
            </div>
            <div class="inputtext">
                <p>Телефон</p>
                <input type="tel" name="phone" id="" pattern="\+7\s?[0-9]{10,12}" maxlength="13"  title="+79374176134">
            </div>
            <div class="inputtext">
                <p>Пол</p>
                <select >
                <option value="" hidden disabled selected>Выбрать</option>
                <option value="Мужской">Мужской</option>
                <option value="Женский">Женский</option>
               
                </select>
            </div>
            <div class="inputtext requir">
                <p>Группа клиентов <span class="required">*</span></p>
                <select required="" class="requir">
                <option value="" hidden disabled selected>Выбрать</option>
                <option value="VIP">VIP</option>
                <option value="Проблемные">Проблемные</option>
                <option value="ОМС">ОМС</option>
                </select>
            </div>
            <div class="inputtext">
                <p>Лечащий врач</p>
                 <select>
                <option value="" hidden disabled selected>Выбрать</option>
                <option value="Иванов">Иванов</option>
                <option value="Захаров">Захаров</option>
                <option value="Чернышева">Чернышева</option>
                </select>
            </div>
            <div class="sendsms">
                
                <input type="checkbox" name="sendsms" value="">Не отправлять смс
            </div>
        </div>

        <div class="section">
            <h2>Адрес</h2>
            <div class="inputtext"> 
                <p>Индекс</p>
                <input type="text" name="index" id="" pattern="[0-9]{6,6}" maxlength="6"  title="543434">
            </div>
            <div class="inputtext">
                <p>Страна</p>
                <input type="text" name="country" id="" pattern="[A-Za-zА-Яа-яЁё\s]{3,30}" title="Россия">
            </div>
            <div class="inputtext">
                <p>Область</p>
                <input type="text" name="area" id="" pattern="[A-Za-zА-Яа-яЁё\s]{3,30}" title="Пензенская">
            </div>
            <div class="inputtext">
                <p>Город <span class="required">*</span></p>
                <input  class="requir" type="text"  name="city" id="" required pattern="[A-Za-zА-Яа-яЁё\s]{2,30}" title="Набережные Челны">
            </div>
            <div class="inputtext">
                <p>Улица</p>
                <input type="text" name="street" id="" pattern="[A-Za-zА-Яа-яЁё\s]{2,30}" title="Карпинского">
            </div>
            <div class="inputtext">
                <p>Дом</p>
                <input type="text" name="house" id="" pattern="[0-9A-Za-zА-Яа-яЁё]{1,3}" title="2а">
            </div>       
        </div>

         <div class="section">
            <h2>Паспорт</h2>
            <div class="inputtext">
                <p>Тип документа <span class="required">*</span></p>
                <select required="" class="requir">
                <option value="" hidden disabled selected>Выбрать</option>
                <option value="Паспорт">Паспорт</option>
                <option value="Свидетельство о рождении">Свидетельство о рождении</option>
                <option value="Вод. удостоверение">Вод. удостоверение</option>
                </select>
            </div>
            <div  class="inputtext">
                <p>Серия</p>
                <input type="text" name="series" id="">
            </div>
            <div class="inputtext">
                <p>Номер</p>
                <input type="text" name="number" id="">
            </div>
            <div class="inputtext">
                <p>Кем выдан</p>
                <input type="text" name="organization" id="">
            </div>
            <div class="inputtext">
                <p>Дата выдачи <span class="required">*</span></p>
                <input class="requir" type="date" name="street" id="" required pattern="[0-9]{2}\.[0-9]{2}\.[0-9]{4}" title="12.04.2020">
            </div>                     
        </div>
        

             <input type="submit" >
         </form>
    </div>
</template>


<script>
export default {
    
}
</script>




<style lang="sass">
h1
    margin-bottom: 70px
.allsections
    background-color: #fff
    color: #202020
    text-align: center
    display: block


.section
   margin: 10px auto
   max-width: 600px
   padding-left: 9px
   padding-right: 9px
   padding-top: 7px
   background: #eee
   border-radius: 10px 

   flex-wrap: wrap
   justify-content: center
   padding-bottom: 10px
.inputtext input
   margin: 10px 0
   margin-bottom: 28px
   font-size: 120%
   padding: 0 0px
   padding-left: 10px
   width: 70%
   height: 40px
   border-radius: 20px
   transition: 200ms
.inputtext input:focus
    width: 90%
    background-color: #ddd
    transition: 200ms


    border-radius: 0px
.inputtext p
   text-size: 20px
   padding-left: 15%
   text-align: left
select
  -moz-appearance: none
  -webkit-appearance: none
  appearance: none
  font-size: 120%
  width: 70%
  height: 40px
  border-radius: 20px
  padding-left: 10px
  border: 0px
select:focus
  border-radius: 0px

.sendsms
    text-size: 20px
    padding-left: 15%
    text-align: left
    margin-top: 20px

input[ type="submit"]
   width: 23%
   height: 40px 
   margin-top: 30px
   margin-bottom: 40px
   border-radius: 20px
input[ type="submit"]:active, input[ type="submit"]:focus 
  outline: none


input[class="requir"]:valid, input[type="date"]:valid, select[class="requir"]:valid 
  border: 2px solid black
  background: #b2dfbe


.required  
    color: red 
</style>

