# My-project

## Отчет о состоянии эксплуатируемого оборудования (СостояниеЭксплуатируемогоОборудования.dt)

В компании используется оборудование, имеющее ограничения к эксплуатации. Для каждого устройства устанавливается срок годности и срок использования. Срок годности считается с момента приобретения оборудования и указывается в документе поступления, а срок эксплуатации с момента его ввода в эксплуатацию и указывается непосредственно для оборудования и не меняется. 
- Поступление оборудования отражается документом «Приходная накладная». 
- Через некоторое время оборудование вводится в эксплуатацию документом «Ввод в эксплуатацию».

При передаче оборудования в эксплуатацию в первую очередь передается оборудование, у которого минимальный срок годности. 
- В документе «Ввод в эксплуатацию» указывается перечень и количество передаваемого оборудования. 
- При проведении должна происходить проверка на наличие оборудования и его срок годности. В том случае, если срок годности истек или оборудования недостаточно, документ не проводится и выдается соответствующее сообщение.

- Раз в месяц формируется регламентный документ «Выбытие оборудования», который при проведении проверяет эксплуатируемое оборудование и, если оно негодно, то списывает его. При проверке определяется, вышел ли срок эксплуатации устройства с момента его ввода в эксплуатацию. Если срок эксплуатации истек или истек срок годности, то оборудование должно быть списано. 
- Кроме того, этот же документ должен списывать еще не введенное в эксплуатацию оборудование, но срок годности, которого уже истек.
- Учет оборудования в разрезе складов не ведется. Себестоимость оборудования рассчитывается как средняя.
- Необходимо создать отчет о состоянии эксплуатируемого оборудования на выбранную дату.

Состояние оборудования в эксплуатации на 31.01.2010

<img width="516" alt="Отчет_СостояниеЭксплуатируемогоОборудования" src="https://github.com/user-attachments/assets/4be92eb6-c4b6-4b47-ab63-bf390cc0b203" />

## Отчет о состоянии взаиморасчетов (Отчет_СостояниеВзаиморасчетов.dt)

Компания занимается оптовой торговлей. Взаиморасчёты с поставщиками ведутся в разрезе соглашений об условиях закупок. Поступление денежных средств поставщику отражается документом «Расход денег», приход товаров — документом «Приходная накладная». 

- И в документе «Расход денег», и в документе «Приходная накладная» может быть указано только одно соглашение — в реквизите шапки.
Когда в документе «Расход денег» указано соглашение, необходимо проверить сумму поставок по этому соглашению. Если была поставка, то происходит погашение задолженности. Если сумма платежа превышает сумму поставки, то оставшиеся деньги должны быть зачтены как аванс. Аванс числится просто за контрагентом, без учёта соглашения. Если соглашение в документе «Расход денег» не указано, то погашаются задолженности по соглашениям в порядке их даты оплаты, дата оплаты указывается в соглашении. Когда сумма платежа больше всех долгов по поставке, оставшаяся сумма также засчитывается как аванс.

- При проведении документа «Приходная накладная» необходимо производить проверку авансов. В случае если аванс есть, необходимо его погасить. Оставшаяся сумма должна быть учтена как долг по соглашению по поставке. Весь учёт ведётся одновременно в трёх валютах: рубли, доллары и евро. При проведении документов курс указывается непосредственно в самом документе. Возникновение курсовых разниц при поставке и оплате не предполагается.

- Учёт остатков номенклатуры не ведётся.

- Необходимо предоставить пользователю возможность самостоятельно добавлять к поставщикам произвольный набор дополнительных характеристик. Этот механизм должен быть реализован с помощью плана видов характеристик. Сами характеристики в настройках отчёта должны быть отображены как реквизиты поставщика.

- Необходимо создать отчёт по состоянию взаиморасчётов по регионам на дату, где регион — это характеристика.

  ![2025-02-23_23-22-30](https://github.com/user-attachments/assets/4d9959f1-36fd-474a-b3d0-8f3b45947bcc)
  
- Дата отчёта должна задаваться пользователем напрямую в форме отчёта. В печатной форме заголовок и шапка отчёта должны соответствовать заданию.


