# Тестирование банковского ПО (Banking domain applications/BFSI)

Банковские приложения (Сектор BFSI или Banking, Financial Services, and Insurance - банковские, финансовые услуги и страхование) являются одними из самых сложных приложений в современной индустрии разработки и тестирования программного обеспечения. Что делает банковские приложения такими сложными? Какой подход следует использовать для тестирования сложных рабочих процессов, связанных с банковскими приложениями? Банковские приложения напрямую связаны с конфиденциальными финансовыми данными. Все операции, выполняемые банковским программным обеспечением, должны выполняться без сбоев и ошибок. Банковское ПО выполняет различные функции, такие как перевод и внесение средств, запрос баланса, история транзакций, вывод средств и так далее. Тестирование банковского приложения гарантирует, что эти действия не только хорошо выполняются, но и остаются защищенными от хакеров.

![https://www.softwaretestinghelp.com/wp-content/qa/uploads/2011/06/Functions-of-Banks.png](https://www.softwaretestinghelp.com/wp-content/qa/uploads/2011/06/Functions-of-Banks.png)

Давайте сначала разберемся с характеристиками банковского приложения:

* Многоуровневая функциональность для поддержки тысяч одновременных пользовательских сеансов;
* Крупномасштабная интеграция. Как правило, банковское приложение интегрируется с множеством других приложений;
* Сложные бизнес-процессы;
* Обработка в режиме реального времени и пакетная обработка (Real-Time and Batch processing);
* Высокая скорость транзакций в секунду;
* Безопасные транзакции;
* Надежный раздел отчетности для отслеживания повседневных транзакций;
* Строгий аудит для устранения проблем клиентов;
* Массивная система хранения;
* Управление аварийными ситуациями/восстановлениями.

Что делает банковские приложения такими сложными?

* Банковское программное обеспечение в основном имеет дело с конфиденциальными финансовыми данными, поэтому работа программного обеспечения должна быть безошибочной и безопасной;
* Разработчики предпочитают сложный дизайн для разработки этих приложений, чтобы гарантировать, что приложение работает безопасным образом;
* Банковское дело - это постоянно меняющийся мир. Банковское дело сегодня доступно для клиентов с использованием различных каналов, таких как обычные отделения, банкоматы, онлайн-банкинг и обслуживание клиентов;
* С появлением технологий многие кошельки наводнили рынки, которые подключаются к банковским системам для финансовых транзакций;
* Ожидается, что банковские услуги будут работать 24\*7 с высокой производительностью. Обновления программного обеспечения, мгновенные исправления и т. д. не должны повлиять на эту доступность;
* На банковский мир также сильно влияют постоянные изменения, вносимые правительством в виде банковских правил. Любые изменения в структуре налогообложения повлияют и на банковскую систему;
* Банковская система также должна быть современной в том, что касается новых технологий. Аналитика данных, такая как обработка больших данных, и получение информации из больших данных с помощью науки о данных (Data Science), становятся все более популярными в банковском мире.

Когда мы говорим о тестировании банковских приложений, требуется методология сквозного тестирования (End to End Testing methodology), включающая несколько методов тестирования программного обеспечения, чтобы гарантировать:

* Полный охват всех банковских рабочих процессов (banking workflows) и бизнес-требований (Business Requirements);
* Функциональный аспект приложения;
* Аспект безопасности приложения;
* Целостность данных (Data Integrity);
* Параллелизм (Concurrency);
* Пользовательский опыт.

**Banking App Testing Workflow**

Типичные этапы тестирования банковских приложений показаны в приведенном ниже рабочем процессе. Мы обсудим каждый этап индивидуально. Это модель Waterfall для тестирования приложения.

![https://www.softwaretestinghelp.com/wp-content/qa/uploads/2011/06/Testing-Banking-Applications.jpg](https://www.softwaretestinghelp.com/wp-content/qa/uploads/2011/06/Testing-Banking-Applications.jpg)

**1. Сбор требований**: этап сбора требований включает в себя документирование требований либо в виде функциональных спецификаций (Functional Specifications), либо в виде вариантов использования (Use Cases). Требования собираются в соответствии с потребностями клиентов и документируются банковскими экспертами или бизнес-аналитиками. Эксперты участвуют в написании требований по более чем одной теме, поскольку банковское дело само по себе имеет несколько поддоменов, и одно полноценное банковское приложение будет интегрировать все эти домены. Например, банковское приложение может иметь отдельные модули для переводов, кредитных карт, отчетов, ссудных счетов, оплаты счетов, торговли и т. д.;

**2. Обзор требований**: результаты сбора требований проверяются всеми заинтересованными сторонами, такими как QA, руководители разработки и бизнес-аналитики. Они перепроверяют, чтобы ни существующие бизнес-процессы, ни новые рабочие процессы не нарушались. Все требования проверены и утверждены. Последующие действия и пересмотры документов требований выполняются на основе того же;

**3. Подготовка бизнес-сценария**: на этом этапе QA составляют бизнес-сценарии (Business Scenarios) из документов с требованиями (requirement documents - Functions Specs or Use Cases); Бизнес-сценарии разработаны таким образом, что охватывают все бизнес-требования. Бизнес-сценарии - это сценарии высокого уровня без каких-либо подробных шагов. Кроме того, эти бизнес-сценарии проверяются бизнес-аналитиками, чтобы убедиться, что все бизнес-требования выполнены. BA легче просматривать сценарии высокого уровня, чем просматривать подробные тестовые случаи низкого уровня. Например, клиент, открывающий срочный депозит в интерфейсе цифрового банкинга, может быть бизнес-сценарием. Точно так же у нас есть различные бизнес-сценарии, связанные с созданием банковского счета, онлайн-депозитами, онлайн-переводами и т. д.;

**4. Функциональное тестирование**: на этом этапе выполняется функциональное тестирование и выполняются обычные действия по тестированию программного обеспечения, такие как:

* **Подготовка тестовых случаев** (Test Case Preparation): на этом этапе тестовые случаи создаются на основе бизнес-сценариев, один бизнес-сценарий приводит к нескольким положительным и отрицательным тестовым случаям;
* **Обзор тестовых случаев** (Test Case Review): обзоры, сделанные коллегами-инженерами по обеспечению качества;
* **Выполнение тестовых случаев** (Test Case Execution): выполнение тестового набора.

Функциональное тестирование банковского приложения сильно отличается от обычного тестирования программного обеспечения. Поскольку эти приложения работают с деньгами клиентов и конфиденциальными финансовыми данными, их необходимо тщательно протестировать. Ни один важный бизнес-сценарий не должен оставаться незамеченным. Кроме того, ресурс QA, который тестирует приложение, должен иметь базовые знания в банковской области.

**5. Тестирование баз данных**: банковское приложение включает в себя сложные транзакции, которые выполняются как на уровне пользовательского интерфейса, так и на уровне базы данных, поэтому тестирование базы данных так же важно, как и функциональное тестирование. База данных сложна и представляет собой совершенно отдельный слой в приложении, поэтому ее тестирование проводится специалистами по базам данных. Оно использует такие методы, как:

* Загрузка данных;
* Миграция базы данных;
* Тестирование схемы БД и типов данных;
* Тестирование правил;
* Тестирование хранимых процедур и функций;
* Тестирование триггеров;
* Целостность данных.

Основная цель тестирования базы данных состоит в том, чтобы убедиться, что:

* Приложение может хранить и извлекать данные из базы данных без потери данных;
* Завершенные транзакции должны быть зафиксированы, а прерванные транзакции должны быть возвращены обратно, чтобы избежать любых несоответствий в сохраненных данных;
* Доступ к базе данных и базовым таблицам разрешен только авторизованным приложениям и пользователям.

В основном существует три способа тестирования базы данных:

* Структурное тестирование: включает в себя тестирование объектов базы данных, таких как базы данных, схемы, таблицы, представления, триггеры, элементы управления доступом и т. д. Обеспечение синхронизации типов данных в таблицах с соответствующими переменными в приложении. Проверка данных и ссылочной целостности в таблицах. Например, поле суммы в приложении должно иметь в таблице тип данных decimal/float. Чтобы соответствовать этим стандартам, пользователям следует предоставить средства управления доступом через представления;
* Функциональное тестирование: включает в себя тестирование баз данных, которые удовлетворяют требованиям пользователя. Есть два способа добиться этого: тестирование черного ящика и тестирование белого ящика. Например, когда мы делаем онлайн-перевод денег, счет отправителя должен быть списан, а счет получателя должен быть зачислен на ту же сумму. Если транзакция завершается неудачей, вся транзакция должна быть отменена, а счет отправителя не должен дебетоваться или кредитоваться обратно;
* Нефункциональное тестирование: включает в себя нагрузочное и стресс-тестирование и оптимизацию производительности. Нагрузочное тестирование помогает определить максимальное количество транзакций, которые могут выполняться одновременно, не влияя на производительность базы данных. Например, на основе результатов нагрузочного и стресс-тестирования банковские приложения могут решить добавить больше ресурсов в свое приложение в часы пик и сократить ресурсы в нерабочее время. Это помогает банку оптимально использовать ресурсы и экономить деньги.

**6. Тестирование безопасности**: тестирование безопасности обычно является последним этапом цикла тестирования. Обязательным условием для начала тестирования безопасности является завершение функционального и нефункционального тестирования. Тестирование безопасности является одним из основных этапов всего цикла тестирования приложений, поскольку на этом этапе обеспечивается соответствие приложения федеральным и отраслевым стандартам. Из-за характера данных, которые они несут, банковские приложения очень чувствительны и являются главной целью для хакеров и мошеннических действий. Тестирование безопасности гарантирует, что приложение не имеет таких веб-уязвимостей, которые могут раскрыть конфиденциальные данные злоумышленнику. Это также гарантирует, что приложение соответствует таким стандартам, как OWASP. На этом этапе основной задачей является сканирование всего приложения, которое выполняется с помощью [различных инструментов](https://www.softwaretestinghelp.com/webinspect-alternatives/). После завершения сканирования публикуется отчет о сканировании. В этом отчете ложные срабатывания отфильтровываются, а остальные уязвимости сообщаются команде разработчиков, чтобы они могли приступить к устранению проблем в зависимости от серьезности каждой проблемы. На этом этапе также проводится тестирование на проникновение, чтобы выявить распространение ошибок. Необходимо проводить тщательное тестирование безопасности на разных платформах, в сетях и ОС. Несколько других используемых ручных инструментов для тестирования безопасности: Paros Proxy, Http Watch, Burp Suite и Fortify. Основная цель тестирования безопасности - выявить любые уязвимости, которые могут быть в программном приложении.

Тестирование безопасности проверяет приложение на:

* Любую внешнюю атаку или попытку взлома приложения со злым умыслом;
* Любую лазейку в программном приложении может быть использована, что приведет к потере данных или денежных средств;
* Любую уязвимость в сети, серверах или рабочих станциях, на которых размещено приложение.

Ниже приведены различные типы тестирования безопасности:

* **Тестирование уязвимостей** (Vulnerability Testing): разрабатывается и выполняется автоматизированная программа для проверки на наличие различных уязвимостей;
* **Сканирование безопасности** (Security Scanning): этот вариант вращается вокруг исследования уязвимостей сети и системы, тем самым предоставляя решения для снижения связанного с этим риска;
* **Тестирование на проникновение** (Penetration Testing): этот вариант тестирования безопасности имитирует попытку взлома для захвата уязвимостей и лазеек, которые могли бы дать хакеру доступ к базе данных или данным приложения;
* **Аудит безопасности** (Security Audit): это включает в себя аудит приложения и связанных сетей на предмет любых нарушений безопасности;
* **Оценка риска** (Risk Assessment): выполняется анализ для оценки уровня риска в случае, если уязвимость или лазейка используются со злым умыслом. Такой риск можно разделить на низкий, средний и высокий. В зависимости от уровня риска группа тестирования рекомендует надлежащие меры для снижения или предотвращения риска;
* **Этический взлом** (Ethical Hacking): выполняется организацией в своих системах для выявления лазеек, которые могут быть использованы в ее приложении или сети. Цель этого вида взлома не состоит в том, чтобы украсть или нанести ущерб приложению или сети;
* **Оценка состояния** (Posture Assessment): это комплексная оценка, включающая сканирование безопасности, оценку рисков и взлом с соблюдением этических норм;
* **SQL-инъекция**: SQL-инъекция может использоваться для получения доступа к базе данных сервера. Тестирование выполняется, чтобы убедиться, что код работает правильно, выполняя запросы в базе данных на основе следующих входных данных от пользователя: Скобки, Апострофы, Запятые, Кавычки.

**Другие этапы тестирования BFSI приложений**

Помимо вышеуказанных основных этапов, могут быть задействованы различные этапы, такие как интеграционное тестирование, тестирование удобства использования, пользовательское приемочное тестирование и тестирование производительности.

**Примеры тестов для банковского приложения**

* Для нового филиала (?New Branch):
  * Создайте новый филиал с допустимыми и недействительными тестовыми данными;
  * Создайте новый филиал без данных;
  * Создайте новый филиал с существующими данными;
  * Проверьте параметры сброса и отмены;
  * Обновите сведения о филиале с допустимыми и недействительными тестовыми данными;
  * Обновите сведения о филиале с помощью существующих тестовых данных;
  * Проверьте, можно ли сохранить новый филиал;
  * Убедитесь, что опция отмены работает;
  * Проверьте удаление филиала с зависимостями и без них;
  * Проверьте, работает ли опция поиска филиалов.
* Для новой роли:
  * Создайте новую роль с допустимыми и недействительными тестовыми данными;
  * Создайте новую роль без данных;
  * Проверьте, можно ли создать новую роль с существующими тестовыми данными;
  * Проверьте описание роли и тип роли;
  * Убедитесь, что опция отмены и сброса работает;
  * Проверьте процесс удаления роли с зависимостью и без нее;
  * Проверьте ссылки на странице сведений о роли.;
  * Проверьте вход администратора без тестовых данных;
  * Проверьте все домашние ссылки для роли администратора;
  * Убедитесь, что администратор может изменить пароль с допустимыми и недействительными тестовыми данными;
  * Убедитесь, что администратор успешно вышел из системы.
* Для Клиента и Банкира:
  * Убедитесь, что все ссылки посетителей и клиентов работают правильно;
  * Проверьте вход клиента с действительными и недействительными тестовыми данными;
  * Проверьте логин клиента без каких-либо данных;
  * Проверьте логин банкира без каких-либо данных;
  * Проверьте логин банкира с действительными или недействительными тестовыми данными%
  * Проверьте, смог ли клиент и банкир успешно выйти из системы.
* Для новых пользователей:
  * Проверьте, можно ли создать нового пользователя с допустимыми и недействительными тестовыми данными;
  * Создайте нового пользователя с существующими тестовыми данными филиала;
  * Убедитесь, что опция отмены и сброса работает правильно;
  * Обновите сведения о пользователе, указав действительные и недействительные тестовые данные;
  * Проверьте удаление нового пользователя;
  * Проверьте, можно ли верифицировать нового пользователя;
  * Проверьте обязательные входные параметры;
  * Проверьте дополнительные входные параметры;
  * Проверьте, можно ли создать пользователя без необязательных параметров.
* Для создания новой учетной записи:
  * Создайте новую учетную запись с действительными и недействительными данными пользователя;
  * Убедитесь, что сведения о пользователе могут быть обновлены;
  * Проверьте, можно ли сохранить нового пользователя;
  * Создайте новую учетную запись с существующими данными пользователя;
  * Убедитесь, что пользователь может внести сумму во вновь созданную учетную запись (и обновить баланс);
  * Проверьте, может ли пользователь снять сумму с новой учетной записи (после внесения депозита и обновления баланса);
  * В случае заработной платы учетная запись проверяет название компании и другие данные, предоставленные пользователем;
  * Проверьте, указан ли номер основной учетной записи в случае дополнительной учетной записи;
  * Проверьте данные пользователя, указанные в случае текущей учетной записи;
  * Проверьте предоставленное доказательство для совместного счета в случае совместного счета;
  * Проверьте, можете ли вы поддерживать нулевой баланс на вашем счете заработной платы;
  * Проверьте, можете ли вы поддерживать нулевой баланс или минимальный баланс для счета, не связанного с зарплатой;
  * Убедитесь, что новый пользователь смог успешно выйти из системы.
* Для сетевого банковского приложения (Net Banking Application):
  * пользователь может открыть сайт банка;
  * все ссылки на сайте работают;
  * пользователь может создать новую учетную запись;
  * Проверьте, может ли пользователь войти в систему с допустимым и недействительным именем пользователя и паролем.
  * Проверьте, что если имя пользователя или пароль пусты при входе в систему, пользователю не должно быть разрешено войти в систему, и должно отображаться предупреждающее сообщение;
  * Проверьте, разрешено ли пользователю изменять пароль;
  * Если введено неверное имя пользователя или пароль, будет показано соответствующее сообщение об ошибке;
  * Пользователям с неверным паролем не разрешается входить в систему;
  * Убедитесь, что после неоднократных попыток входа с неправильным паролем пользователю должно быть показано сообщение об ошибке и он заблокирован;
  * Проверьте, может ли пользователь выполнять некоторые основные транзакции;
  * Убедитесь, что пользователь может добавить получателя с допустимыми и недействительными данными;
  * Проверьте, может ли пользователь удалить получателя;
  * Убедитесь, что пользователь может совершать транзакции для вновь добавленного получателя;
  * После транзакции проверьте, были ли обновлены учетные записи пользователя и получателя;
  * Проверьте, может ли пользователь ввести сумму в десятичном виде (4.50);
  * Убедитесь, что пользователь не может вводить отрицательные числа в поле суммы;
  * Проверьте, разрешено ли пользователю совершать транзакции с минимальным балансом или без него;
  * Проверьте, может ли пользователь создать новый RD;
  * Убедитесь, что отображается правильное сообщение в случае транзакции, выполненной с недостаточным балансом;
  * Проверьте, запрашивается ли у пользователя подтверждение перед выполнением какой-либо транзакции;
  * Убедитесь, что квитанции о подтверждении предоставлены для каждой успешной транзакции;
  * Проверьте, может ли пользователь переводить деньги на несколько счетов;
  * Проверьте, может ли пользователь отменить транзакцию;
  * Убедитесь, что данные учетной записи также отражают выполненные финансовые операции;
  * Убедитесь, что функция тайм-аута реализована;
  * Убедитесь, что в случае истечения времени сеанса пользователь должен снова войти в систему;
  * Убедитесь, что установлен правильный тайм-аут сеанса в случае бездействия;
  * Убедитесь, что при выполнении транзакции пользователь переведен в безопасный режим;
  * Убедитесь, что пользователь смог успешно выйти из системы;
  * Проверьте параметры поиска и сброса.

Источники:

* [How To Test Banking Domain Applications: A Complete BFSI Testing Guide](https://www.softwaretestinghelp.com/testing-banking-applications/)

Доп. материал:

* [How To Test Investment Banking Application (With 34+ Important Test Scenarios)](https://www.softwaretestinghelp.com/how-to-test-investment-banking-application/)
* [How To Test Retail Banking System](https://www.softwaretestinghelp.com/how-to-test-retail-banking-system/)