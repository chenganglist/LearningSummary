����ָ��        

ϵͳ��������        

���ѹ���������        

�ػ�/��������        

Linux�ܵ�        

Linux���������        

vimʹ��        

�û����û������        

�ļ�Ȩ�޹���        

���ԣ�http://www.weixuehao.com/archives/25        



����ָ��        

ls����        ��ʾ�ļ���Ŀ¼        

     -l           �г��ļ���ϸ��Ϣl(list)        

     -a          �г���ǰĿ¼�������ļ���Ŀ¼���������ص�a(all)        

mkdir         ����Ŀ¼        

     -p           ����Ŀ¼�����޸�Ŀ¼���򴴽�p(parent)        

cd               �л�Ŀ¼        

touch          �������ļ�        

echo            �����������ݵ��ļ���        

cat              �鿴�ļ�����        

cp                ����        

mv               �ƶ���������        

rm               ɾ���ļ�        

     -r            �ݹ�ɾ������ɾ����Ŀ¼���ļ�        

     -f            ǿ��ɾ��        

find              ���ļ�ϵͳ������ĳ�ļ�        

wc                ͳ���ı����������������ַ���        

grep             ���ı��ļ��в���ĳ���ַ���        

rmdir           ɾ����Ŀ¼        

tree             ���νṹ��ʾĿ¼����Ҫ��װtree��        

pwd              ��ʾ��ǰĿ¼        

ln                  ���������ļ�        

more��less  ��ҳ��ʾ�ı��ļ�����        

head��tail    ��ʾ�ļ�ͷ��β����        

ctrl+alt+F1  ������ȫ��ģʽ        

         

ϵͳ��������        

stat              ��ʾָ���ļ�����ϸ��Ϣ����ls����ϸ        

who               ��ʾ���ߵ�½�û�        

whoami          ��ʾ��ǰ�����û�        

hostname      ��ʾ������        

uname           ��ʾϵͳ��Ϣ        

top                ��̬��ʾ��ǰ�ķ���Դ��������Ϣ        

ps                  ��ʾ˲�����״̬ ps -aux        

du                  �鿴Ŀ¼��С du -h /home���е�λ��ʾĿ¼��Ϣ        

df                  �鿴���̴�С df -h ���е�λ��ʾ������Ϣ        

ifconfig          �鿴�������        

ping                ����������ͨ        

netstat          ��ʾ����״̬��Ϣ        

man                ��������ˣ�������  �磺man ls        

clear              ����        

alias               ������������ �磺alias showmeit="ps -aux" ��������ʹ        ��unaliax showmeit        

kill                 ɱ�����̣���������ps �� top����鿴���̵�id��Ȼ������kill����ɱ��        ���̡�        

         

���ѹ���������        

gzip��        

bzip2��        

tar:                ���ѹ��        

     -c              �鵵�ļ�        

     -x              ѹ���ļ�        

     -z              gzipѹ���ļ�        

     -j              bzip2ѹ���ļ�        

     -v              ��ʾѹ�����ѹ������ v(view)        

     -f              ʹ�õ���        

����        

tar -cvf /home/abc.tar /home/abc              ֻ�������ѹ��        

tar -zcvf /home/abc.tar.gz /home/abc        ���������gzipѹ��        

tar -jcvf /home/abc.tar.bz2 /home/abc      ���������bzip2ѹ��        

��Ȼ��������ѹ������ֱ���滻���������  tar -cvf  / tar -zcvf  / tar -jcvf �еġ�        c�� ���ɡ�x�� �Ϳ����ˡ�        

         

�ػ�/��������        

shutdown        

     -r             �ػ�����        

     -h             �ػ�������        

     now          ���̹ػ�        

halt               �ػ�        

reboot          ����        

         

Linux�ܵ�        

��һ������ı�׼�����Ϊ��һ������ı�׼���롣Ҳ���ǰѼ��������������ʹ�ã���һ���������ǰһ������Ľ����        

����grep -r "close" /home/* | more       ��homeĿ¼�������ļ��в��ң�����clo        se���ļ�������ҳ�����        

         

Linux���������        

dpkg (Debian Package)�����ߣ����������.deb��׺�����ַ����ʺ�ϵͳ��������������¡�        

���簲װtree����İ�װ�����Ƚ�tree.deb����Linuxϵͳ�С���ʹ���������װ��        

sudo dpkg -i tree_1.5.3-1_i386.deb         ��װ���        

sudo dpkg -r tree                                     ж�����            

         

ע����tree.deb����Linuxϵͳ�У��ж��ַ�ʽ��VMwareTool��ʹ�ù��ط�ʽ��ʹ��winSCP���ߵȣ�            

APT��Advanced Packaging Tool���߼�������ߡ����ַ����ʺ�ϵͳ�ܹ����ӻ������������        

��Ȼ��treeΪ��        

sudo apt-get install tree                         ��װtree        

sudo apt-get remove tree                       ж��tree        

sudo apt-get update                                 �������        

sudo apt-get upgrade                

         

��.rpm�ļ�תΪ.deb�ļ�        

.rpmΪRedHatʹ�õ������ʽ����Ubuntu�²���ֱ��ʹ�ã�������Ҫת��һ�¡�        

sudo alien abc.rpm        

         

vimʹ��        

vim����ģʽ������ģʽ������ģʽ���༭ģʽ��ʹ��ESC��i�����л�ģʽ��        

����ģʽ�£�        

:q                      �˳�        

:q!                     ǿ���˳�        

:wq                   ���沢�˳�        

:set number     ��ʾ�к�        

:set nonumber  �����к�        

/apache            ���ĵ��в���apache ��n������һ����shift+n��һ��        

yyp                   ���ƹ�������У���ճ��        

h(����һ���ַ���)��j(��һ�С�)��k(��һ�С�)��l(����һ���ַ���)        

         

�û����û������        

/etc/passwd    �洢�û��˺�        

/etc/group       �洢���˺�        

/etc/shadow    �洢�û��˺ŵ�����        

/etc/gshadow  �洢�û����˺ŵ�����        

useradd �û���    passwd �û���  usermod �޸��û�        

userdel �û���    adduser �û���        

groupadd ����     groupdel ����   groupmod �޸��û�        

chown ---change own ---�޸��û���        

chmod  ---change mod ---�޸��ļ�����        

Linuxͨ���ļ����Ժ��û�������ʵ��Ȩ�޹���        
��ÿһ���ļ���Բ�ͬ���û����û��Ĵ���Ȩ�޲�һ��        
����Linuxһ�н��ļ����Ӷ�������ʵ����LinuxȨ�޹���        
����ͨ���鿴Linux��ͬĿ¼�²�ͬ�ļ������ԣ��˽���һ����        

passwd root     ��root��������        

su root        

su - root         

/etc/profile     ϵͳ��������        

bash_profile     �û���������        

.bashrc              �û���������        

su user              �л��û������������ļ�.bashrc        

su - user            �л��û������������ļ�/etc/profile ������bash_profile            

�����ļ����û����û���        

sudo chown [-R] owner[:group] {File|Directory}        

���磺����jdk-7u21-linux-i586.tar.gzΪ���������û�hadoop����hadoop        

Ҫ���л����ļ��������û����顣����ʹ�����        

sudo chown root:root jdk-7u21-linux-i586.tar.gz        

         

�ļ�Ȩ�޹���        

���ֻ���Ȩ��        

R           ��         ��ֵ��ʾΪ4        

W          д         ��ֵ��ʾΪ2        

X           ��ִ��  ��ֵ��ʾΪ1        



��ͼ��ʾ��jdk-7u21-linux-i586.tar.gz�ļ���Ȩ��Ϊ-rw-rw-r--        

-rw-rw-r--һ��ʮ���ַ����ֳ��ĶΡ�        

��һ���ַ���-����ʾ��ͨ�ļ������λ�û����ܻ���֡�l�����ӣ���d����ʾĿ¼        

�ڶ����ĸ��ַ���rw-����ʾ��ǰ�����û���Ȩ�ޡ�   ��������ֵ��ʾΪ4+2=6        

�������߸��ַ���rw-����ʾ��ǰ�������Ȩ�ޡ�      ��������ֵ��ʾΪ4+2=6        

�ڰ˾�ʮ���ַ���r--����ʾ�����û�Ȩ�ޡ�              ��������ֵ��ʾΪ2        

���Բ������ļ���Ȩ������ֵ��ʾΪ662         

����Ȩ��        

sudo chmod [u�����û�  g������  o�����û�  a�����û�]  [+����Ȩ��  -����Ȩ��]  [r          w  x]   Ŀ¼��         

���磺��һ���ļ�filename��Ȩ��Ϊ��-rw-r----x�� ,��Ȩ��ֵ��Ϊ"-rwxrw-r-x"������ֵ��ʾΪ7        65        

sudo chmod u+x g+w o+r  filename        

��������ӿ�������ֵ��ʾ        

sudo chmod 765 filename        

         