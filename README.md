# excelcompleximport
复杂格式excel转换，excel 转换成 xml

```配置xml样例
<packinglist>
    <head replicate="false">
        <INVOICEDATE start-tag="INVOICE DATE*" data-formatter="$.Split(':')[1]"/>
        <PAYMENT start-tag="PAYMENTWAY*" data-default="OA 60" data-formatter=""/>
        <REFERENCENO start-tag="REFERENCE NO*" data-offset="c:3"/>
        <NAME start-tag="NAME*" data-formatter="$.Split(':')[1]"/>
        <ADDRESS1 start="A9" data-formatter="$.Split(':')[1]"/>
        <ADDRESS1 start="H9" data-formatter="$.Split(':')[1]"/>
    </head>
    <detail replicate="true" start-tag="PLANT" end-tag="TOTAL">
        <PLANT data-field="PLANT" data-type="string" />
        <STORAGE data-field="STORAGE" data-type="string" />
        <SHIP_NO data-field="SHIP_NO" data-type="string" />
        <FAC_SO_NO data-field="FAC_SO_NO" data-type="string" />
        <LINE data-field="LINE" data-type="string" />
        <DN_NO data-field="DN_NO" data-type="string" />
        <DN_ITEM data-field="DN_ITEM" data-type="string" />
        <PART_NO data-field="PART_NO" data-type="string" />
        <QTY data-field="QTY" data-type="string" />
        <PQTY data-field="箱数" data-type="string" />
        <GWT data-field="毛重" data-type="string" />
        <CKG data-field="长-宽-高" data-type="string" />
        <TQTY data-field="托数" data-type="string" />
        <CUST_PN data-field="CUST_PN" data-type="string" />
    </detail>
</packinglist>
```
