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
git log  �鿴�޸ļ�¼
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



�½���֧�����л�����֧
���������޸ĵ����ݸ��µ���֧��������ʱmaster��֧���ݱ��ֲ���
��dev�������ɣ���ȷ��������л���master��֧�����ϲ�dev��֧����ʱ���߿����ͬ����״̬
��֧����
git checkout -b dev    ������Ϊdev�ķ�֧(-b��ʾ�������л�)
= git branch dev  +  git checkout dev   ������֧dev + �л���֧

git branch �鿴��ǰ��֧
git checkout master  �л�Ϊmaster��֧���л���֧ǰȷ���ѽ����������ݸ��µ�git����ȥ
git log ��ʾ Endʱ������CTRL+C or ����q��
git merge  --no-ff -m ��explanation��  dev  
��ָ����dev��֧�ϲ�����ǰ��֧(��master��֧)��ȥ���������ͬ��
git branch -d dev ɾ��dev��֧
git branch -D dev ǿ��ɾ��dev��֧
git log --graph   �ɲ鿴��֧�ϲ�ͼ
branch test1 and test2
git stash ����ǰ�����ֳ��������������������ָ��ټ�����һ��������ʱ�½���֧ȥ��bug
git stash list �鿴����Ĺ����ֳ�
git stash pop = git stash apply + git stash drop �ָ���ɾ��stash
git stash apply stash@{0} ѡ��ָ����stash�ָ�