1.��Ŀ���
  (1)ģ�⵱������Ҫ�Ĺ���
  (2)��Ҫ�������¹���ģ��
     a.��Ʒ���ģ�� main
     b.���ﳵģ�� cart
     c.�û�����ģ�� user
     d.��������ģ�� order
  (3)��Ҫ������Щ����
     a.Struts2���
     b.JDBC+dbcp���ӳ�
            ���ӳغô�:
        1.����Ƶ������������connection
     	2.��connection������һ��������Χ��
     	    ��֤�������ȶ�.
     c.�ͻ��˲���jQuery+Ajax
   (4)���ݿ����(����ʹ��PowerDesign����)
      a. d_user��
                �洢�û�ע�����Ϣ.
      b. d_receive_address��
                �洢�û�ʹ�ù����ջ���ַ.
      c. d_category��
                �洢��Ʒ�����Ϣ
      d. d_product��
                �洢�������Ͳ�Ʒ�Ĺ�����Ϣ
      e. d_book��
                 �洢ͼ���Ʒ��������Ϣ
      f. d_category_product��
                 �洢���Ͳ�Ʒ֮��İ�����ϵ
      g. d_order��
                �洢������Ϣ��.
      h. d_item��
                �洢������ϸ��.
2.���̽ṹ
   ���ֲ� : JSPҳ�� �漰��ǩ,OGNL���ʽ,jQuery,Ajax
   ���Ʋ� : ʹ��Struts2������,�漰struts.xml����
   ҵ��� : Action���
   ���ݷ��ʲ� : DAO���
  srcԴ����ṹ����:
  com.tarena.dang.action
  com.tarena.dang.action.user �û�ģ��Action
  com.tarena.dang.action.order ����ģ��Action
  com.tarena.dang.action.main ��Ʒ���ģ��Action
  com.tarena.dang.action.cart ���ﳵAction
  com.tarena.dang.dao  �ӿ�
  com.tarena.dang.dao.impl ʵ����
  com.tarena.dang.entity ʵ����
  com.tarena.dang.util ������
  com.tarena.dang.interceptor ������
  Struts�����ļ��ṹ����:
     struts.xml(������)
        --struts-main.xml(��Ʒ���ģ������)
        --struts-order.xml(����ģ������)
        --struts-user.xml(�û�����ģ������)
        --struts-cart.xml(���ﳵģ������)
  WebRootĿ¼�ṹ����:
   /WebRoot/main/ ��Ʒ���JSPĿ¼
   /WebRoot/cart/ ���ﳵJSPĿ¼
   /WebRoot/order/ ����JSPĿ¼
   /WebRoot/user/  �û�����JSPĿ¼
   /WebRoot/common/ ҳüҳ��Ŀ¼
   /WebRoot/css/  ��ʽ�ļ�Ŀ¼
   /WebRoot/js/   �ű��ļ�Ŀ¼
   /WebRoot/images/ JSP��ͼƬĿ¼
   /WebRoot/productImages/ ��ƷͼƬĿ¼
  
  
  http://localhost:8080/dang/user/login.action
  
   
   



   
   
   
     
     
     
     
     
     
     
     