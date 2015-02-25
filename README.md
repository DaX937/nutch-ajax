Nutch AJAX page Fetch, Parse, Index Plugin
==============

### ��Ŀ���

����Apache Nutch 2.3��Htmlunit, Selenium WebDriver�������չ��ʵ�ֶ���AJAX��������ҳ�������ҳ������ץȡ���Լ��ض�������Ľ�����������

According to the implementation of Apache Nutch 2.X, we can't get dynamic HTML information from fetch pages including AJAX requests as it will ignore all AJAX requests.

This plugin will use Htmlunit and Selenium WebDriver to fetch whole page content with necessary dynamic AJAX requests. 

It developed and tested with Apache Nutch 2.3, you can try it on other Nutch 2.X version or refactor the source codes as your design.

### ��Ҫ����

* **�����HTMLҳ��ץȡ**: ���ڳ��������������û��AJAX���Ե�ҳ�����ֱ����Nutch�Դ���protocol-http���ץȡ��

* **�����AJAXҳ��ץȡ**: ���ھ��󲿷�����jQuery ajax���ص�ҳ�棬����ֱ����htmlunit��չ���ץȡ��

* **�����AJAX����ҳ��ץȡ**: �����Ա�/��è��ҳ������˶��ص�Kissy Javascript�����Ŀǰ����htmlunit�޷���ȷ����������˶�����β���Ч�ʵ�һЩ��Selenium WebDriver��ʽʵ��ҳ������ץȡ��

* **����ҳ�������AJAX����ҳ��ץȡ**: �����Ա�/��è����Ʒ����ҳ������ҳ�����������Ʒ������Ϣ�ļ��أ�ͨ��Htmlunit��Selenium WebDriver��չ�������ʵ�ִ���ҳ������ץȡ��

### ���з�ʽ

������Ŀ���ڹٷ���Apache Nutch 2.3Դ�����֮����Ӳ����������ã����з�ʽ�͹ٷ�ָ�ϱ���һ�£�������ο���http://wiki.apache.org/nutch/

ͬʱ���̴������ύ��Eclipse�Ĺ��������ļ�������ֱ��import Eclipse��Run��Debug���У�Nutch������Ivy�������������ɲ���ANT Build��ʽ������Eclipse IDE��װApache Ivy IDE������й��̱������С�

![snapshot](http://git.oschina.net/xautlx/nutch-ajax/raw/master/snapshot/eclipse-run.jpg)

![snapshot](http://git.oschina.net/xautlx/nutch-ajax/raw/master/snapshot/storage-data.jpg)

![snapshot](http://git.oschina.net/xautlx/nutch-ajax/raw/master/snapshot/parse-data.jpg)

### ��չ���˵��

* **protocol-s2jh**: ����Htmlunit��Selenium WebDriverʵ�ֵ�AJAXҳ��Fetcher���

* **parse-s2jh**: ����XPath����ҳ��Ԫ������; �־û��������Ľṹ�����ݣ���MySQL��MongoDB��; ���ڸ���������AJAXҳ�涨���ж�ҳ�������ɵĻص��ж��߼�

* **index-s2jh**: ׷��������Ҫ���⴫�ݸ�SOLR��������������; �趨����Ҫ������ҳ�����;

### ���˵��

* ��ԴЭ��

����Ŀ���д���������Դ���ڱ�����ʶ����Ŀ��Դ��Ϣ�Լ���֤���Ա���Ŀ���з���Ȩ��������Ϊ��ǰ���£����������ⷽʽ����ʹ�ã���Դ���ǿ�Դ����ҵ������ҵ��

* �շѷ���

�����ϣ���ṩ����Apache Nutch/Solr/Lucene��ϵ�м����Ķ��Ƶ���չʵ��/������ѯ����/��ҵ���ָ��/���ο�����Ŀָ�����κ�����Ȥ�ĺ�����ʽ��������ϵ E-Mail: xautlx@hotmail.com �� QQ: 2414521719 (��Q��ע����nutch/solr/lucene) Э���շѷ���[������ϵ��ʽˡ��ֱ���ṩ��ѵļ�����ѯ��ѯ�ʣ�������Ŀ���κμ��������Issue��������ֱ���ύ����Ŀվ�����ʻ�Gitƽ̨��Issue]
 
