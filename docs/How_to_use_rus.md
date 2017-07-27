# ��� ������������
** �����! ���������� ���������� �� ������ �� �����, � ����� ����������! �����! **
## ��� ��������? ##
��� ����������� ��������� ������. � ����� *** instabot/examples/ *** ��������� ������� ��� ������
## ��� ��������� ������? ##
�������� ��������� ������, ��� ������ ������� *** cd *** ��������� � ������� �������, � ������ *** instabot/examples ***. 
�������� 
``` python 
python name.py param
```
��� *** name *** � �������� �������, *** param *** � ����������� �������� ��� ������� �������. �� ��� ���� �������� ����� ��������
## ��� � ���� ������ ��� ������ ������� ��������� ������� ��������? ##
��������� ������, ������ 
``` python
python name.py
```
������ �����������, ���� ��� ����������� ���������� � ���� ��� �� ���� �����.
������. 
��������� ������ 
``` python
python like_hashtags.py. 
``` 
������ ��������������� � ������� ��� ���������: 
``` python
error: the following arguments are required: hashtags.
```
�� ���� �� ������ ���� ����� �������. 
���������� ������: 
``` python
python like_hashtags.py follow
```
## �� ��������
*** multi_script_CLI.py *** � ������, ������� �������� ��� �������. ��� ������ ��� ������� ��� ����� ���������� ��������� ������. ��������� ������� �������� � ����� *** setting.txt ***.
����� ����� ������� �����: *** hashtag_file.txt, users_file.txt, whitelist.txt, blacklist.txt, comment.txt ***.
## 24/7
��, ���� ������, ������� ������������� �������� ����������� � �������� ������������ �����, � ����� ������� ���������� �� �������� � ���������� �����. ��� ��� ��������� ������ - *** ultimate.py ***, ������� ��������� � ����� *** /instabot/examples/ultimate/ ***. � ����� ����� ��������� ������ ��������� ����� ��� ������ �������. � ���� ������ ������ ����� �������� ����� ������ � ����� ������.
## ������ ������
����� ���� ������, ������� ����� �������� �������������, �� ���� ������ ����� ����������� �� �����. ���� ������ � *** ultimate.py *** � ����� *** /instabot/examples/ultimate_schedule/ ***. �� ������ ������� ��� ����� ���������� � ��������� ��� � ��� ����� �����, ��� ��� ������������ ����������� � ������ ������ ����.
## ��� ��������� ��������� ������
��� ����, ����� ��� ������� �� ��� ������� - ����� ��������� ������
������, �������� ��� ����� ������� ���������� �� ������� ������ ������. �������� ����� ����� � ��������.
�������� *** like_hashtags.py *** ��� ������ ���������� ���������. ������� ����� ������� (�������� ��� ��� ������ ���������)
``` python
bot = Bot()
bot.login(username=args.u, password=args.p,
          proxy=args.proxy)
```
������ � ������
``` python
bot = Bot()
```
��� ����� �������� � ������� ��������. ���� ���������� �������� *** like_delay ***. ����� ��������� ����� ��������� �������� 60, ��� ��� ��� �����, ����� ������ ������ ������ ���������� �� �������.
� ����� ��� ����� ��������� ��� ���
``` python
bot = Bot(like_delay=60)
bot.login(username=args.u, password=args.p,
          proxy=args.proxy)
```
### ������ ����������

| ��������| �������� | ������ |
| ------------- |:-------------:| ------:|	
| proxy | Proxy for Instabot | None|	
| max_likes_per_day| How many likes the bot will perform per day| 1000|
| max_unlikes_per_day | How many medias the bot will unlike in a day| 1000|	
| max_follows_per_day| Max number of follow per day| 350|
| max_unfollows_per_day| Max number of follow per day| 350|
| max_comments_per_day| Max number of comments per day| 100|
| max_likes_to_like| If the media has more likes then this value - it will be ignored and not be liked | 200|
| filter_users | Filter users if True | True|
| max_followers_to_follow| If the user has more followers than this value - the user will not be followed or liked. | 2000|
| min_followers_to_follow| If the user has fewer followers than this value - the user will not be followed or liked.| 10|
| max_following_to_follow| If the user has more followings than this value - the user will not be followed or liked.| 10000|
| min_following_to_follow| If the user has fewer followings than this value - the user will not be followed or liked.| 10|
| max_followers_to_following_ratio| if the user's followers/following is greater than this value - the user will not be followed or liked.| 10|
| max_following_to_followers_ratio| if user's following/followers is greater than this value - he will not be followed or liked.| 2|
| min_media_count_to_follow| If the user has fewer media count than this value - the user will not be followed. | 3|
|max_following_to_block|If the user have a following more than this value - the user will be blocked in blocking scripts because he is a massfollower| 2000|
| max_likes_to_like | Max number of likes that can media have to be liked | 100 |
| like_delay | Delay between likes in seconds| 10|
| unlike_delay | Delay between unlikes in seconds | 10|
| follow_delay | Delay between follows in seconds| 30|
| unfollow_delay | Delay between unfollows in seconds| 30|
| comment_delay | Delay between comments in seconds|  60|
| whitelist | Path to the file with users that shouldn't be unfollowed| "whitelist.txt"|
| blacklist | Path to the file with users that shouldn't be followed, liked or commented | "blacklist.txt"|
| comments_file | Path to the comments database | "comments.txt" |
| stop_words| A list of stop words: don't follow a user if they have any of these stop words in their description| ['shop', 'store', 'free']|



