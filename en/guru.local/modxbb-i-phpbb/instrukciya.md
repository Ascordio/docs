
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<h2>MODxBB и phpBB: Инструкция</h2>

<h2 class="page-header">Руководство по установке и настройке конфигурации MODxBB</h2>
<p>Добро пожаловать в документацию MODxBB. Эта документация включена в пакет MODxBB, также вы можете ознакомиться с ней в Интернете на сайте <a rel="nofollow" title="MODxBB.net/documentation" href="http://modxbb.net/documentation">modxbb.net/documentation</a></p>
<p>Данное руководство связано с оглавлением на правой стороне, так же там есть информация о дате создания и последней модификации для каждой страницы. Эта информация позволяет быстро проверить, когда страница была обновлена. Кроме того, я создал файл CSS для вывода на печать, который должен пригодиться тем, кто предпочитает читать документацию на бумаге.</p>
<h2 class="page-header">1. Документация MODxBB</h2>
<h2 class="page-header">1.1 MODxBB</h2>
<p>MODxBB интегрирует MODX и PhpBB друг в друга при сохранении масштабируемости</p>
<p>MODX является высоко настраиваемой системой управления контентом, которая также может быть использована в качестве основы для управления контентом</p>
<p>PhpBB это очень мощная система управления веб-форумами, которая широко используется в качестве коммуникационной платформы, однако, она имеет значительный потенциал</p>
<p>Администраторы, которые хотели бы использовать MODX PhpBB сталкиваются с проблемой, что пользователям придется дважды регистрироваться и поддерживать два аккаунта для одного сайта. Одна из главных целей MODxBB заключается в решении этой проблемы путем интеграции обеих систем друг в друга</p>
<p>Это гораздо больше, чем просто мост для учетных записей пользователей. Используя MODxBB, разработчик может получить доступ к обоим интерфейсам на любой PhpBB странице, а также на любой странице MODX <br>Подробнее о MODxBB и его особенности можно прочитать в статье <a rel="nofollow" href="http://www.modxbb.net/index.php?id=48" target="_blank">Добро пожаловать в MODxBB</a> на <a rel="nofollow" href="http://modxbb.net/" target="_blank">modxbb.net</a>.</p>
<h2 class="page-header">1.2 Об этой документации</h2>
<p>Этот документ получился гораздо подробнее, чем первоначально планировалось. Он предназначен для ознакомления даже неопытными пользователями, однако, необходимо отметить, что чем глубже ваши знания о (X) HTML, CSS и PHP, тем больше вы можете получить от использования MODxBB</p>
<p>В этом руководстве рассматриваются все возможные типы установки, следовательно, вам не потребуется все это изучать. Дополнительные разделы начинаются с уведомления о том, когда они необходимы для чтения</p>
<p>Несмотря на не слишком простую установку и настройку, после установки у вас не должно возникнуть проблем в использовании MODxBB. В будущих версиях планируется сделать интерфейс для упрощения установки и настройки.</p>
<h2 class="page-header">1.3 Дополнительные учебники</h2>
<p>Более подробные руководства, советы и примеры по различным темам, будут добавляться на блог <a href="http://modxbb.net/" target="_blank">modxbb.net</a> позже.</p>
<h2 class="page-header">2. Установка</h2>
<h2 class="page-header">2.1 Требования к установке</h2>
<ul>
	<li>MODX Evolution 1.0.0 - 1.0.15 рекомендуется: <a rel="nofollow" title="MODX Evolution download" href="http://modx.com/evolution/download/">1.0.7</a></li>
	<li>phpBB 3.0.4 - 3.0.11 • рекомендуется: <a rel="nofollow" title="phpBB download" href="http://www.phpbb.com/downloads">3.0.11</a></li>
	<li>MODxBB 0.9.5 (входит в комплект поставки)</li>
	<li>Веб-сервер для работы phpBB и MODX.</li>
</ul>
<h2 class="page-header">2.2 Установка MODX</h2>
<p>Установите MODX Evolution. Если такая установка уже существует, настоятельно рекомендуется обновить до последней версии, если вы еще не сделали этого. На странице <a rel="nofollow" href="http://modx.com/evolution/download/" target="_blank">загрузки MODX</a> вы можете узнать, какая версия является последней и загрузить ее при необходимости</p>
<p>В процессе установки, вы должны поставить сайт в "Оффлайн" режим: Инструменты -&gt; Конфигурация -&gt; Статус сайта, выберите 'Оффлайн'.</p>
<h2 class="page-header">2.3 Установка phpBB</h2>
<p>Создайте в корне вашего сайта папку 'forum' (форум может быть установлен в любую папку, но папка 'forum' рекомендуется). Если у вас уже установлен phpBB, посетите <a rel="nofollow" href="http://www.phpbb.com/downloads" target="_blank">страницу загрузки PhpBB</a>, чтобы убедиться, что у вас последняя версия.</p>
<p>Настоятельно рекомендуется расположить папку 'forum' в корне сайта. Установка форума в другую папку должна выполняться только опытными пользователями. Если вы хотите, чтобы ваш форум был интегрирован в шаблон сайта, как это сделано на <a rel="nofollow" href="http://modxbb.net/forum" target="_blank">MODxBB.net</a>, вам необходимо настроить основные шаблоны phpBB (overall_header и overall_footer). О том, как это делается, подробно описано в соответствующей ветке форума <a rel="nofollow" href="http://www.phpbb.com/community/viewtopic.php?f=74&amp;t=963325" target="_blank">phpBB.com</a>.</p>
<p><span class="text-bold">СОВЕТ:</span> Некоторые браузеры имеют полезные инструменты (Firebug в Firefox или DragonFly в Opera), что может вам пригодиться при оформлении стиля вашего форума, потому что они облегчают работу с CSS. Я также рекомендую бесплатную утилиту <a rel="nofollow" title="Colour To HTML" href="http://www.matthewhipkin.co.uk/colourtohtml.php">Colour To HTML</a> , так как она экономит массу времени при подборе необходимого цвета, которую требуется изменить в другой. (Color-picker -&gt; find in CSS)</p>
<p>Еще один совет, который может сэкономить вам много времени: overall_header.html и overall_footer.html вместе взятые являются полной HTML-страницей. Вы можете их объединить (например в редакторе) для редактирования, и разделить снова, после того, как закончите редактирование.</p>
<p>Вставка PhpBB шаблона как часть шаблона или документа MODX, кстати, теоретически возможна, но не разумна.</p>
<h2 class="page-header">2.4 Установка MODxBB</h2>
<p><span class="text-bold">ПРИМЕЧАНИЕ:</span> function_user.php входящий в пакет MODxBB содержит исправление ошибки в строке 2186 которое решает вопрос об аватарах галереи, не сортируемых должным образом. Я добавил это наряду с возможностью MODxBB использовать аватары галереи.</p>
<h2 class="page-header">2.4.1 Резервное копирование</h2>
<p><span class="text-bold"><span style="color: #ff0000;">ВАЖНО:</span></span> Сделайте резервное копирование всех файлов, которые будут заменены или отредактированы. Чтобы узнать, какие файлы были изменены при полной установке MODxBB, читайте страницу <span style="text-decoration: underline;">Список файлов</span> или просмотрите папку "Documents" включая подпапки.</p>
<p>При желании вы можете сделать копию всего сайта, но это не обязательно. Файлы, которые будут перезаписаны (быстрая установка) или отредактированы (выборочная установка) можно найти в папке Documents в архиве MODxBB.</p>
<h2 class="page-header">2.4.2 Минимальная установка</h2>
<p>Если все, что вы хотите, это вывести чанки и сниппеты на вашем форуме, просто скопируйте файл modxapi.php (входящий в комплект MODxBB) в корень вашего сайта, и переходите к главе 2.4.6.</p>
<h2 class="page-header">2.4.3 Быстрая установка</h2>
<p>Есть три требования к быстрой установки:</p>
<ul>
	<li>1. PhpBB 3.0.11</li>
	<li>2. MODX 1.0.7 Evo </li>
	<li>3. Ни один из файлов, которые будут заменены не были изменены пользователем до этой установки (если вы не хотите потери внесенных изменений).</li>
</ul>
<p><span class="text-bold"><span style="color: #ff0000;">НЕ ЗАБУДЬТЕ ПРО РЕЗЕРВНОЕ КОПИРОВАНИЕ!</span></span></p>
<p>Просто скопируйте файлы из папки MODxBB\Documents в корень вашего сайта, сохранив структуру папок.</p>
<p><span class="text-bold">ПРИМЕЧАНИЕ:</span> Это предполагает, что ваша папка форум называется "forum". Кроме того, если вы не хотите настроить стиль JOT в стиле MODxBB пропустите папку JOT.</p>
<h2 class="page-header">2.4.4 Выборочная установка</h2>
<p>Выборочная установка необходима, если вы используете устаревшую версию PhpBB или MODX, либо модифицированную версию, которую вы хотите сохранить или просто хотите знать, что было отредактировано при установке.</p>
<p>Я отказался от моего первоначального плана показать все вносимые изменения, назвав номера строк, потому что есть риск вас запутать. В зависимости от версии и количества модификаций добавленных пользователями, отличия в изменениях могут быть слишком велики.</p>
<p>Вместо этого мы будем использовать более безопасный и понятный способ: Посетим <a rel="nofollow" href="http://www.modxbb.net/index.php?id=55" target="_blank">домашнюю страницу WinMerge</a> и скачаем последнюю версию WinMerge. Это отличная бесплатная программа, которая может сравнивать файлы и показывать их различия. Linux и Mac пользователи могут найти альтернативы в <a rel="nofollow" href="http://en.wikipedia.org/wiki/File_comparison" target="_blank">этой статье</a>.</p>
<p>Все, что нужно сделать сейчас, это сравнить файлы в папке "Original" с файлами в папке "Documents". Обратите внимание на различия и их расположение в файле. Не полагайтесь на номер строки! Вместо этого проверьте строки до и после изменений и включите их в то же место файла на вашем веб-сервере.</p>
<p><span class="text-bold">Пример: </span></p>
<p>После установки, запустите WinMerge и выберите в меню Файл -&gt; Открыть, чтобы добавить файл index.php находится в папке "Documents", а также файл, который расположен в папке "Original", которые вы можете найти в архиве MODxBB. Теперь скачайте index.php вашего сайта и включите в него различия двух других файлов, которые показал WinMerge (не забудьте про резервные копии ваших файлов!). Когда закончите, загрузите отредактированный и сохраненный файл index.php в корень вашего сайта. Сделайте то же самое с другими файлами.</p>
<h2 class="page-header">2.4.5 Установка элементов [сниппеты, плагин]</h2>
<p>Установка MODxBB элементов не является обязательной. Вы можете установить их все или только часть. Вы можете пропустить этот раздел, если вам не нужны эти элементы. В следующей таблице перечислены все включенные в комплект MODxBB элементы:</p>
<div class="flip-scroll">
	<table class="table table-bordered table-vcenter flip-content">
		<thead class="flip-content bordered-palegreen">
			<tr><th>Название</th><th>Тип</th><th>Описание</th></tr>
		</thead>
		<tbody>
			<tr>
				<td>LatestTopicsBB</td>
				<td>сниппет</td>
				<td>Отображает последние активные темы форума</td>
			</tr>
			<tr>
				<td>LoginBB</td>
				<td>сниппет</td>
				<td>Регистрация в MODxBB и профиль авторизованного пользователя</td>
			</tr>
			<tr>
				<td>OnlineListBB</td>
				<td>сниппет</td>
				<td>Показывает кто находится на сайте</td>
			</tr>
			<tr>
				<td>PrevPollsBB</td>
				<td>сниппет</td>
				<td>Отображает историю опросов</td>
			</tr>
			<tr>
				<td>SitePollBB</td>
				<td>сниппет</td>
				<td>Выводит PhpBB опросы на любой странице сайта</td>
			</tr>
			<tr>
				<td>PluginBB</td>
				<td>плагин</td>
				<td>
					<p>Связывает профили пользователей PhpBB с профилями веб-пользователей MODX</p>
				</td>
			</tr>
		</tbody>
	</table>
</div>
<p>Более подробное описание, включая скриншоты можно найти на <a rel="nofollow" href="http://modxbb.net/" target="_blank">MODxBB.net</a></p>
<p>Для установки любоuj из приведенных выше cybggtnjd, войдите в ваш менеджер MODX, перейдите по ссылке: Элементы -&gt; Управление Элементами -&gt; Сниппеты и нажмите кнопку "Новый сниппет". Название такое же, как имя файла или как в приведенном выше списке. Для описания введите <span class="text-bold"> 0.9.5 </span> , а затем введите описание из таблицы выше. Описание поможет распознать фрагмент, номера версии нужны для отличия от возможных будущих версий</p>
<p>Теперь вставьте содержание соответствующего файла в код сниппета, файлы находятся в папке "Elements" в пакете MODxBB. Не забудьте сохранить сниппет!</p>
<p>Для установки плагина PluginBB перейдите в Элементы -&gt; Управление Элементами -&gt; Плагины и нажмите кнопку "Новый плагин"</p>
<p>Задайте название, описание и код как в примере выше.<br>Теперь нажмите на "Системные события" и активируйте флажки "OnUserFormRenter" и "OnWUsrFormRender". Сохраните плагин.</p>
<h2 class="page-header">2.4.6 Настройка шаблонов phpBB</h2>
<p>Тот, кто хочет разработать свой стиль форума настроив дизайн в соответствии с дизайном сайта, должен пройти шаги, описанные в разделе 2.3</p>
<p>Следующий шаг необходим только тем, кто хочет разместить MODX элементы (сниппеты, чанки) или сообщения об ошибках MODX на форуме. Если вам это не нужно, вы можете перейти в раздел 3. Конфигурация</p>
<p>Во-первых, откройте файл overall_header.html. Это может быть сделано в PhpBB администраторской панели управления (Общие -&gt; Стили -&gt; Шаблоны), либо путем поиска файлов в папке forum\styles\ВашаТема\template (при условии, что форум находится в папке "forum" и у вас установлена нужная тема). Затем добавьте следующие строки в начале этого файла:</p>
<pre class="brush: php;">&lt;?php
	if (!defined('ADMIN_START')){
		require_once($phpbb_root_path . '../modxapi.php');
	}
	else {
		require_once($phpbb_root_path . '../../modxapi.php');
	}

	global $modx;
	$modx = new MODxAPI();
	$modx-&gt;connect();
	$modx-&gt;getSettings();
?&gt;</pre>
<p>Следующий шаг необходим только если вы хотите отображать сообщения об ошибке MODX на вашем форуме PhpBB.</p>
<p>Добавьте следующие строки в нижней части шаблона:</p>
<pre class="brush: php;">&lt;?php
	$MODx_output = '';
	global $MODx_output;
	if ($MODx_output) {
		echo $MODx_output;
	}
?&gt;</pre>
<p>Теперь найдите файл overall_footer.html (находится в той же папке) и добавьте следующие строки в верхней части:</p>
<pre class="brush: php;">&lt;?php
	global $modx;
?&gt;</pre>
<h2 class="page-header">3. Конфигурация</h2>
<h2 class="page-header">3.1 Настройка MODX</h2>
<p>Если вы сделали минимальную установку, вы можете перейти к разделу <a title="chapter 3.1.4" href="#c3-1-4">3.1.4</a>.</p>
<h2 class="page-header">3.1.1 Отключите WebLogin</h2>
<p>Вы должны избавиться от регистрационной формы WebLogin если она у вас используется, потому что PhpBB заботится о регистрации пользователей и передает пользовательские данные в MODX. Для обеспечения авторизации и регистрации на ваших страницах MODX используйте сниппет LoginBB, который включен в пакет MODxBB.</p>
<h2 class="page-header">3.1.2 Добавьте новое поле для Jot в таблицу MODX</h2>
<p>Это необходимо, если вы хотите настроить JOT в стиле MODxBB, как показано на главной странице и на форуме MODX</p>
<p>Войдите в свой ​​PhpMyAdmin, выберите базу данных MODX и нажмите на modx_web_user_attributes (у вас может быть другой префикс, не modx_). Теперь нажмите на "Структура" (верхняя строка), перейдите к строке "Добавить" (в зависимости от темы PhpMyAdmin она может также быть в верхней части). Добавьте 1 поле, щелкните переключатель "В конец таблицы" нажмите ОК</p>
<p>Теперь введите следующие значения:</p>
<div><span class="text-bold">Поле:</span> postcount</div>
<div><span class="text-bold">Тип:</span> Int (11)</div>
<div><span class="text-bold">По умолчанию:</span> 0 [выбрать "Как определено:" из выпадающего списка]</div>
<div><span class="text-bold">Комментарии:</span> jot comments</div>
<p>Нажмите кнопку Сохранить.</p>
<h2 class="page-header">3.1.3 Выберите аватар по умолчанию для гостя в Jot</h2>
<p>То же самое применимо и здесь: Это только необходимо если вы хотите использовать Jot в стиле MODxBB</p>
<p>Откройте chunk.comment.inc.html в папке jot\templates (тот, который вы загрузили ранее) и заменить <span class="text-bold">assets/images/YourDefaultAvatar.png</span> в строке 8 на URL к аватару по умолчанию, и <span class="text-bold">assets/images/YourGuestAvatar.png</span> в строке 10 на URL к аватару по умолчанию для гостей</p>
<p>Вы можете загружать аватары в папку assets или хранить их в другом месте, однако, чтобы сохранить согласованность, я рекомендую добавить аватар группе для гостей (анонимных пользователей) и для группы зарегистрированных пользователей в PhpBB и использовать их</p>
<p>Вы можете сделать это в администраторской панели PhpBB (ACP) -&gt; Пользователи и группы -&gt; Управление группами - -&gt; Настройки.</p>
<h2 id="c3-1-4">3.1.4 Добавьте ссылку на форум</h2>
<p>Чтобы показать ссылку на Ваш форум в списках, созданных сниппетом Wayfinder и т.д. (например в карте сайта), Вы должны создать веб-ссылку на ваш форум. Это может быть сделано в менеджере MODX. Для получения дополнительной информации о том, как создать веб-ссылку, читайте документацию MODX или спрашивайте на форуме.</p>
<h2 class="page-header">3.2 Конфигурация phpBB</h2>
<h2 class="page-header">3.2.1 Включите PHP в шаблонах</h2>
<p>Это необходимо только, если вы хотите показать элементы MODX или сообщения об ошибках на вашем форуме, в противном случае переходите к главе 3.2.2 .</p>
<p>Войдите в администраторскую панель (АСР) PhpBB и нажмите на кнопку "Безопасность" в "Конфигурация сервера" на вкладке Общие. Выделите "Разрешить PHP в шаблонах:" и выберите "Да". Нажмите кнопку Отправить. Этот шаг необходим для обработки команд MODX, которые были ранее добавлены в шаблон PhpBB.</p>
<p><span class="text-bold"><span style="color: #ff0000;">ВНИМАНИЕ:</span></span> Не загружайте и не запускайте ненадежные PhpBB темы в то время, когда этот параметр включен! Вы должны загрузить темы только из phpBB.com или других надежных источников.</p>
<h2 class="page-header">3.2.2 Убрать привязку форм к гостевым сессиям</h2>
<p>Этот шаг необходим только если вы хотите, чтобы гости имели возможность проголосовать на ваших страницах MODX при использовании сниппета SitePollBB</p>
<p>Идите на ту же страницу, как в 3.2.1 (ACP -&gt; Общие -&gt; Конфигурация сервера -&gt; Безопасность) и найдите пункт "Привязать формы к гостевым сессиям:" (должен быть внизу). Измените значение на "Нет" и нажмите кнопку Отправить.</p>
<h2 class="page-header">3.2.3 Перекомпилировать старые шаблоны</h2>
<p>Этот шаг необходим, если вы планируете добавить чанки или сниппеты к PhpBB. Это гарантирует, что ваш форум распознает и отобразит визуальные изменения, сделанные вашими элементами MODX на форуме</p>
<p>Войдите в свой ​​PhpBB АСР. На вкладке Общие выделите вкладку "Конфигурация сервера" и нажмите "Нагрузка на сервер". Теперь нужно найти "Перекомпилировать старые шаблоны:" измените на "Да" и нажмите кнопку Отправить.</p>
<h2 class="page-header">3.2.4 Добавление элементов MODX в шаблон PhpBB</h2>
<p>Теперь вы можете добавлять команды для запуска MODX элементов (чанки, сниппеты) на форуме. Они могут быть добавлены в любой из шаблонов, которые мы редактировали в разделе 2.4.6 или любой другой шаблон, который принадлежит этой же теме, тем не менее, я рекомендую добавить их в нижней части overall_header.html</p>
<p>Это эффективный способ показа объявлений на вашем форуме (но лично я не люблю объявления на форумах), как на MODxBB.net или чего-нибудь еще, что Вы хотите, чтобы ваши читатели форума увидели. Примеры: Чтобы запустить чанк MODX, который отображает объявления на вашем форуме, откройте overall_header.html расположенный в папке forum\styles\ВашаТема\template и добавьте следующие строки в нижней части шаблона, между тегами PHP, которые мы добавляли в разделе 2.4.6 :</p>
<pre class="brush: php;">echo $modx-&gt;getChunk('Announcement');</pre>
<p>Где 'Announcement' имя вашего чанка.</p>
<p>Если вы добавляли в шаблон строки для вывода ошибок MODX, это будет выглядеть так:</p>
<pre class="brush: php;">&lt;?php
	echo $modx-&gt;getChunk('Announcement');
	$MODx_output = '';
	global $MODx_output;
	if ($MODx_output){
		echo $MODx_output;
	}
?&gt;</pre>
<p>или так:</p>
<pre class="brush: php;">&lt;?php
	echo $modx-&gt;getChunk('Announcement');
?&gt;</pre>
<p>Вы можете также добавить это где-либо еще в пределах шаблона или в любом другом шаблоне.</p>
<p>Чтобы вставить сниппет, используйте:</p>
<pre class="brush: php;">echo $modx-&gt;runSnippet('SomeSnippet');</pre>
<p>Если сниппет имеет параметры, мы поступим следующим образом:</p>
<pre class="brush: php;">echo $modx-&gt;runSnippet("MySnippet", array('column'=&gt;'3', 'tpl'=&gt;'MyTemplate')</pre>
<p>Где 'column' и 'tpl' - параметры, а '3' и 'MyTemplate' - значения.</p>
<p>Для наглядности, вы можете создать массив:</p>
<pre class="brush: php;">$parameters['column']=3;
$parameters['tpl']=MyTemplate;
echo $modx-&gt;runSnippet('snippet_name', $parameters);</pre>
<p>При размещении в шаблоне, не забывайте PHP теги:</p>
<pre class="brush: php;">&lt;?php
	$parameters['column']=3;
	$parameters['tpl']=MyTemplate;
	echo $modx-&gt;runSnippet('snippet_name', $parameters);
?&gt;</pre>
<h2 class="page-header">3.3 Конфигурация элементов MODxBB</h2>
<p>Для настройки поставляемых сниппетов, откройте его и измените переменные в разделе конфигурации. В более поздних версиях вы сможете передавать параметры в сниппет.</p>
<h2 class="page-header">3.3.1 LatestTopicsBB</h2>
<p>Есть три переменные, которые можно настроить в конфигурации этого сниппета. Первая <code>$num_post</code> определяет количество отображаемых статей, которые отображает этот сниппет. Во-вторых, <code>$num_chars</code> определяет количество символов, которые отображаются в каждой статье и, наконец, <code>$DefaultAvatar</code> позволяет установить аватар по умолчанию для пользователей, которые не установили аватар.</p>
<h2 class="page-header">3.3.2 LoginBB</h2>
<p>Есть два параметра, которые вы можете изменить. В качестве значения переменной <code>$phpBB_folder</code> в первом разделе содержатся имя главной папки форума. Если это, в соответствии с рекомендациями, папка «forum», оставьте значение переменной как есть</p>
<p>Для настройки рангов пользователей прокрутите вниз до <code>switch ($phpBB_rank)</code>. Здесь перечисленны визуальные отображения рангов, а цифры используются для идентифицирования рангов в PhpBB. Большая часть из этого очевидна, однако, будет статья о MODxBB.net, которая объяснит подробно работу системы рангов и групп в phpBB и MODxBB.</p>
<h2 class="page-header">3.3.3 OnlineListBB</h2>
<p>Этот сниппет также имеет параметр <code>$phpBB_folder</code> в первом абзаце, который должен быть изменен в случае, если папка вашего форума не называется «forum»</p>
<p>Если вы НЕ используете сниппет SitePollBB на той же странице, раскомментируйте, пожалуйста, второй абзац (удалив / * и * / ).</p>
<p>OnlineListBB использует JQuery, чтобы узнать, что это такое и как оно работает читайте документацию JQuery. Пусть вас это не пугает, на самом деле нужно добавить только одну строку, чтобы подключить JQuery, которая выглядит следующим образом:</p>
<pre class="brush: html;">&lt;script type="text/javascript" src="js/jquery-1.5.min.js"&gt;&lt;/script&gt;</pre>
<p>Это предполагает, что вы загрузили JQuery сценарий и скопировали его в папку "js". Имейте в виду, что вам, возможно, не нужно этого делать, если у вас уже есть подключенная библиотека JQuery. Вам также, возможно, придется установить режим совместимости, если вы используете библиотеку MooTools, например.</p>
<h2 class="page-header">3.3.4 PrevPollsBB</h2>
<p>Этот сниппет отображает историю опросов. Он может быть использован в качестве истории для опросов, которые были показаны SitePollBB или отдельно</p>
<p>Если папка вашего форума отличается от папки по умолчанию, вы должны настроить ее и здесь. В первом абзаце найдите <code>$phpbb_root_path</code> и замените «forum» на имя папки вашего форума. Например, если ваша папка называется 'board', замените './forum/' на './board/' </p>
<p>Существуют пять переменных, которые устанавливаются в разделе конфигурации (второй абзац). <code>$forum_ids</code> идентификаторы форумов, из которых необходимо брать опросы, указываются через запятую.</p>
<p><code>$ num_posts</code> определяет максимальное количество отображаемых опросов.</p>
<p><code>$per_page</code> количество опросов на одной странице. Если $per_page будет меньше $num_posts, то сниппет отобразит пагинацию, для перехода между опросами.</p>
<p><code>$page_start</code> стартовая страница при пагинации. Где <code>request_var</code> функция PhpBB, которая позволяет безопасно перейти к значению запроса. Рекомендуется оставить этот параметр без изменений.</p>
<h2 class="page-header">3.3.5 SitePollBB</h2>
<p>Конфигурация этого сниппета находится в файле poll.php , расположенном в папке modxbb, поставляется с пакетом MODxBB.</p>
<h2 class="page-header">3.4 Настройка документов MODxBB</h2>
<h2 class="page-header">3.4.1 poll.php</h2>
<p>Это основной двигатель для сниппета SitePollBB. Он содержит две переменных для его настройки</p>
<p>Измените значение <code>$prevpollID</code> в строке 20, указав ID вашей MODX страницы, которая содержит сниппет PrevPollsBB подключенный к сниппету SitePollBB. Объяснение: Eсть ссылка "Предыдущие опросы" в сниппете SitePollBB, которая определяется здесь.</p>
<p>В строке 54 устанавливаются форум (ы), откуда берутся опросы для размещения на странице MODX, которая содержит SitePollBB. Вы можете выбрать один или несколько</p>
<p>Например, если вы хотите отобразить последние опросы форумов с ID 12 и 13, необходимо изменить строку следующим образом: <code>$CFG['poll_forum'] = array(12,13);</code></p>
<p>В строках 57-59 настраивается отображение BBCode, смайликов и URL-адресов.</p>
<h2 class="page-header">3.4.2 edit.php</h2>
<p>MODxBB поддерживает дополнительные поля PhpBB. Вы можете сделать так (но не обязательно), чтобы они отображались в профиле веб-пользователей MODX</p>
<p>Для этого вам нужно настроить edit.php и signup.php оба расположены в папке modxbb. Пример с "fullname" уже включен туда. Если вы создаете пользовательский профиль в PhpBB с идентификацией по "fullname", вы автоматически получите значение для этого поля из профиля веб-пользователей MODX "Full name". Чтобы создать дополнительное поле, зайдите в АСР, на закладке "Пользователи и группы" нажмите "Дополнительные поля в профиле" в разделе Пользователи</p>
<p>Этот файл управляет изменениями, которые сделаны в PhpBB и передает их в MODX, следовательно, дополнительные поля необходимо ввести отдельно, если вы хотите, чтобы они отобразились в профиле MODX. В строках 38-47 показано как это работает. Префикс <code>pf_</code> всегда добавляется, остальное (здесь «fullname») поле идентификации пользовательского профиля</p>
<p>Подробное руководство о том, как создавать и управлять дополнительными полями, в том числе, как изменить профили веб-пользователей в MODX будет позже опубликовано в блоге MODxBB.net.</p>
<h2 class="page-header">3.4.3 signup.php</h2>
<p>Второй файл, который необходимо изменить, если вы хотите добавить дополнительные поля в MODX и PhpBB является signup.php</p>
<p>Строка 26 содержит пример для «fullname»:</p>
<pre class="brush: php;">$fields["fullname"] = $cp_data['pf_fullname'];</pre>
<p>в этой строке параметру <code>pf_fullname</code> присваивается значение параметра fullname из таблицы MODX. Вы так же можете присвоить это значение любому другому параметру.</p>
<p>В строке 28 значение поля fone таблицы site_web_user_attributes присваивается значению поля user_id таблицы phpbb_users. Я выбрал этот путь для простоты. Можно, конечно, создать поле phpBB_ID в базе данных MODX или использовать любую другую область. Это используется для связи профилей PhpBB и MODX, таким образом, если вы используете другое поле, отличное от поля по умолчанию, нужно настроить плагин PluginBB (просто найти "phone" и заменить на нужное поле).</p>
<p>В строке 29 замените <code>forum/download/file.php?avatar=g2_1266363854.png</code> на URL для аватара по умолчанию (для пользователей, у которых нет аватара).</p>
<p>Если вы не хотите, чтобы новым пользователям отправлялось сообщение с приветствием, поставьте в начале строки 33 две черты //</p>
<h2 class="page-header">3.4.4 welcome.php</h2>
<p>Этот файл содержит текст сообщения, которое отправляется пользователям сразу после регистрации.</p>
<p>Как показано в строке 25, вы можете использовать <code>$BridgeUser</code> в качестве шаблона для ника получателя. Теоретически, можно использовать любые другие параметры, принадлежащие пользователю, значение которых хранится в MODX или PhpBB. Смайлики и BBcode также поддерживаются</p>
<p>В строке 45 <code>$fields["phone"]</code> указывается идентификатор пользователя PhpBB. Если, как это описано в предыдущей главе, вы выбрали другое поле, укажите его вместо "phone"</p>
<p>Остальное должно быть понятным.</p>
<h2 class="page-header">3.4.5 login.php</h2>
<p>Убедитесь в том, что используете одинаковые параметры кодировки для поля username обеих систем (MODX и PhpBB). Рекомендуется кодировка <code>utf8_unicode_ci</code>, однако, если вы решите использовать другую кодировку, ее необходимо изменить в строке 88. Просто замените "utf8_unicode_ci" в этой строке названием вашей кодировки.</p>
<h2 class="page-header">4. Общие советы и примечания</h2>
<h2 class="page-header">4.1 Использование CSS для настройки вывода сниппетов</h2>
<p>Все элементы MODxBB поддерживают CSS и, таким образом, позволяют настраивать вывод. Рекомендуется использовать CSS-сброс, чтобы настроить одинаковое отображение во всех браузерах (это также общие рекомендации CSS, а не только MODxBB).</p>
<p>На странице CSS селекторы перечислены все селекторы, которые находятся в css файле. Эти значения идентичны тем, которые используются на MODxBB.net.</p>
<h2 class="page-header">4.2 Вполне возможно иметь отдельный аватар для блога</h2>
<p>Возможно использовать отдельные аватары для блогов (отличных от аватаров на форуме). То же самое касается любых других данных профиля. Поскольку изменения, которые вносятся в PhpBB в "Панели управления" будут отправлены в MODX, но не наоборот.</p>
<p><span style="color: #ff0000;"><span class="text-bold">ВАЖНО:</span></span> Если вручную внести изменения в административной панели управления АСР (например, имя пользователя), это должно быть сделано вручную и в MODX, так как это еще не автоматизировано в этой версии.</p>
<h2 class="page-header">4.3 MODxBB позволяет настраивать содержание</h2>
<p>Вы можете настроить индивидуальное содержание для каждого пользователя в соответствии с его уровнем или званием, или по другим критериям. Это относится и к свойствам в профиле.</p>
<p><span class="text-bold">Примеры: </span></p>
<p>- Можно создавать контент, который виден только зарегистрированным пользователям.</p>
<p>- Вы можете написать объявление, которое будет показано только пользователям с 1000 или более сообщениями или со специальным званием "Premium User" (специальные звания могут быть созданы в PhpBB ACP).</p>
<p>- Сообщение пользователям, которые празднуют свой день рождения с особым содержанием (например, баннер с поздравлением).</p>
<p>Подробное описание и примеры на эту тему будут размещены в блоге MODxBB.net позже.</p>
<h2 class="page-header">4.4 Система аутентификации</h2>
<p>Некоторые читатели могут спросить, почему бы просто не использовать только систему аутентификации PhpBB, раз PhpBB интегрировано таким образом на страницы MODX. Это действительно возможно, но если вы опустите аутентификацию в MODX, учетные записи пользователей на сайте MODX будет полностью непригодны для некоторых дополнений MODX. Это также включает в себя роли и права созданные в менеджере MODX</p>
<p>Если для вас это не проблема, и вы знакомы с PHP, вам ни что не мешает это использовать. Все что вам нужно это отключение обновления параметров MODX</p>
<p>Я напишу учебник по этой теме, если на него будет спрос.</p>
<h2 class="page-header">4.5 PluginBB</h2>
<p>Это всего лишь полезный инструмент, который может пригодиться в некоторых случаях. Вы можете открыть в окне административной панели MODX профиль phpBB. Если вы предпочитаете открытие в полном окне, просто откройте его в новой вкладке.</p>
<h2 class="page-header">4.6 Журналы MODxBB</h2>
<p>MODxBB генерирует журналы, которые можно прочитать в административной панели MODX (Отчеты -&gt; Просмотр событий). Они окажут, как предполагается, помощь в поиске потенциальных проблем и попыток взлома. Наиболее важная информация показывается, без детального просмотра. Это экономит время и повышает читабельность. Ошибки входа в систему отображаются как «Тип ошибки - IP - Имя пользователя", где P - был введен неправильный пароль, а U - неверное имя пользователя.</p>
<h2 class="page-header">4.7 Защита от спама</h2>
<p>Эта тема непосредственно не связаны с MODxBB и PhpBB. Любой работающий форум, скорее всего, столкнется с проблемой спама. В частности, с начала этого года наблюдается увеличение спам-атак</p>
<p>Существуют различные способы защитить форума от спама. Я первоначально планировал рассказать о некоторых из них здесь, но на phpBB.com уже есть полезные статьи об этом. Таким образом, я просто добавлю ссылки на эти статьи:</p>
<p><a rel="nofollow" href="http://www.phpbb.com/community/viewtopic.php?f=46&amp;t=2122696">Preventing Spam in phpBB3</a> - Большинство из этих методов также применимы и для других платформ.</p>
<p><a rel="nofollow" href="http://www.phpbb.com/community/viewtopic.php?f=46&amp;t=2122697">Spam Discussion</a> - Дополнительные советы.</p>
<h2 class="page-header">4.8 Использование Web2Manager при регистрации веб-пользователей</h2>
<p>Когда пользователь регистрируется, MODxBB создает соответствующую учетную запись веб-пользователя в MODX. Web2Manager очень полезный плагин для управления веб-пользователями. Он также позволяет, создать учетную запись веб-пользователя из существующей учетной записи пользователя MODX. Существующие учетные записи будут обновлены</p>
<p>Последнюю версию можно скачать здесь: <a rel="nofollow" href="http://www.modxbb.net/assets/files/web2manager-0.3.3.zip" target="_blank">Web2Manager-0.3.3.zip</a></p>
<h2 class="page-header">5. Известные проблемы</h2>
<h2 class="page-header"><em>5.1. Двойное голосование</em></h2>
<p><em>В очень редких случаях обновление страницы с опросом может дать возможность проголосовать 2 раза. </em>Это происходит только тогда, когда гости имеют право голоса и гости могут изменить свой выбор и может быть выбрано несколько вариантов ответа. Это очень маловероятно, но не невозможно</p>
<p>Обходной путь: Просто удалите дополнительные опции.</p>
<h2 class="page-header">5.2 Выход из LoginBB</h2>
<p>Выход из системы в сниппете LoginBB перенаправляет на индексную страницу форума вместо возврата на ту же страницу, в отличии от входа в учетную запись, когда пользователь возвращается на ту же страницу.</p>
<p><span class="text-bold">Примечание:</span> Это не ошибка. Чтобы вернуть пользователя на ту же страницу, которую он посетил, прежде чем выйти из системы, пришлось бы изменить файл ядра, в то время как пользователю в большинстве случаев все равно, куда он будет перенаправлен.</p>
<p>Решение: чтобы вернуть пользователя туда, где он находился при выходе из системы, вы должны внести изменения в функцию PhpBB meta_refresh.</p>
<h2 class="page-header">5.3 Теги MODX</h2>
<p>Специальные теги MODX ([~ID~]) не работают на страницах PhpBB. Это может быть исправлено в одной из будущих версий</p>