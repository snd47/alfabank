<template>
 
      <div id="app">
            <header>
                <a>
                    <img src="@/img/logo.png"  alt="Логотип Альфабанк">
                </a>
            </header>

    <main>
      <article>
        <section class="main">
           <h1>Купуй на знижках з кредиткою «Максимум»</h1>
            <ul class="features-list">
                <li class="feature-item">
                    <p>До 200 000 гривень </p>
                    <p>кредитного ліміту</p>
                </li>
                <li class="feature-item">
                    <p>Оплата частинами</p>
                    <p>до 24 місяців під 1,8% 1%*</p>
                </li>
                <li class="feature-item">
                    <p>Cashback до 20%</p>
                    <p>на всі покупки</p>
                </li>
                 <li class="feature-item">
                    <p>До 62 днів</p>
                    <p>пільгового періоду</p>
                </li>
            </ul>
        </section>
        <section class="order-form">
           <h2>Замовити картку</h2>
            <form method="post" action="http://httpbin.org/post" autocomplete="off" @submit="submitted=true" target="_blank">
                          <label>
                            <span>Прізвище</span>
                            <input type="text" name="name" maxlength="30"  pattern="[\p{L}\s]{1,30}" required>
                          </label>
                          <label>
                            <span>Ім'я</span>
                            <input type="text" name="name" maxlength="30"  pattern="[\p{L}\s]{1,30}" required>
                          </label>
                          <label>
                            <span>По батькові</span>
                            <input type="text" name="name" maxlength="30"  pattern="[\p{L}\s]{1,30}" required>
                          </label>
                          
                          
                          <label >
                            <span>Номер мобільного</span>
                            <input type="tel" v-mask="'+38093-###-##-##'"  name="phone" required >
                          </label>
                          
                           <label>
                            <span>ІПН</span>
                            <input type="number"  name="phone" required >
                          </label>

                          <label>
                            
                            <select>
                              <option disabled selected value="worktype">Тип працевлаштування</option>
                              <option value="working">Працюю офіційно</option>
                              <option value="workingblack">Працюю неофіційно</option>
                              <option value="selfworking">Приватний підприємець</option>
                              <option value="notworking">Тимчасово не працюю</option>
                              <option value="retired">Пенсіонер</option>
                              <option value="student">Студент</option>
                            </select>
                          </label>
                          
                          <label class="agree-checkbox">
                            <input type="checkbox" name="check" checked required>
                            <span>Я погоджуюся з <a href="#">умовами оформлення</a> онлайн-заявки</span> 
                           </label>


                          
                          <button class="btn" type="submit" value="Submit" :disabled="submitted">Відправити заявку</button>
                        </form>

        </section>
      </article>  

    </main>
    <footer>
      <div class="footer">
       <ul class="footer-list">
                      <li class="footer-item">
                          <p>Швидке</p>
                          <p>схвалення</p>
                      </li>
                      <li class="footer-item">
                          <p>Безкоштовна</p>
                          <p>доставка</p>
                      </li>
                      <li class="footer-item">
                          <p>Безконтактні</p>
                          <p>оплати</p>
                      </li>
                      
                  </ul>
      </div>
    </footer>

        
      </div>
</template>

<script>

</script>

<style lang='scss'>


 
 
</style>
