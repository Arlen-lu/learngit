cd D:/MyGit   ��λ��git���ַ
pwd  ��ѯ��ǰ·��
mkdir projectname  �½��ļ���
cd projectname ��λ����Ŀ�ļ���
git init    �ڵ�ǰ·���´�������ʼ��Git �ֿ⣬��Ÿ���Ŀ����������
�����Ƚ�git add���ݴ���������git commit���汾����ȥ
git add filename  �ύ����/�޸ĵ��ļ����ݴ���
git commit -m "explanation about what you add"  �������/�޸ĵ��ļ����ݴ����ύ����֧�⣬��������ݴ���
git status   �鿴�ֿ⵱ǰ״̬�����ļ����޸ĵ�
git diff  ��ʾ�ļ��޸ĵľ�������
add log  �鿴�޸ļ�¼
cat filename  �鿴�ļ�����
git reflog �鿴ÿ��ִ�е�����
git checkout -- filename    ���ļ��ص����һ��git commit��git addʱ��״̬��
git reset HEAD filename    ���ݴ������޸Ļ��˵�������
���˰汾��  
git reset --hard HEAD^   ���˵���һ���汾
git reset --hard HEAD~100 ���˵���100���汾
git reset --hard commit_id       ����/���ص���Ӧ�汾(be68Ϊcommit id)
rm filename  ɾ�����������ļ�
git rm filename ɾ���汾���е��ļ�
git checkout -- filename ʹ�ð汾���еİ汾�滻�������İ汾�������汾���е��ļ��ָ�����������
MyGit ������
.gitΪ�汾��

ssh-keygen -t rsa -C "email"   ����SSH����
git remote add origin git@github.com:username/filename.git   �����ؿ������github�Ŀ������
git push -u origin master             �����ؿ�������������͵�Զ�̿���ȥ���״�ָ��Ĭ�Ϸ���������Ҫ���-u
ssh -T git@github.com                                          git����github
git clone git@github.com:username/projectname��¡Զ�̿⵽���ؿ���
ls �鿴��ǰ·���µ��ļ���


��֧����
git checkout -b dev    ������Ϊdev�ķ�֧(-b��ʾ�������л�)
= git branch dev  +  git checkout dev 

git branch �鿴��ǰ��֧
