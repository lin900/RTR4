###5.1��ɫģ��
####Goochģ��

- ����
    - ���淨��n
    - ���߷���v
    - ���շ���l
- ����
    - //��ɫ=�߹�ɫ+(1-�߹�ɫ)(ůɫ+(1-ůɫ)��ɫ)
    - $C~shader~=sC~highlight~+(1-s)(tC~warm~+(1-t)C~cool~)$
    - $C~cool~=(0,0,0.55)+0.25C~surface~$
    - $C~warm~=(0.3,0.3,0)+0.25C~surface~$
    - $C~highlight~(1,1,1)$
    - $t=\frac{(n*l)+1}{2}$
    - $r=2(n*l)n-l$ //l�����n�ķ��䷽�� reflect()
    - $s=clamp((100(r*v)-97))$
    //���Բ�ֵ����lerp(),mix()

###5.2����
- ����
    - $C~shaderd=f~unlit(n,v)+\sum_{i=1}^{n}C~light~i~~f~lit(l~i~,n,v)$
    - $f~unlit~$��ʾ��ȫ���ܹ��յ���ۣ������Ǵ���ɫ�������������ɫ

![gooch](./Images/gooch.png)
