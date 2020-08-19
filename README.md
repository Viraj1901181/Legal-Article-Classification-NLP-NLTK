## Data Overview

The sample folder consists of 3 main data files:
- `article_topic.csv`
- `articles.csv`
- `topic_relationships.csv`

#### articles.csv
Here you will find information on articles content. Columns in `articles.csv` are:

- `article_id` - unique article indentifier
- `title` - articles title
- `body` - articles text (in HTML format)
- `country_desc` - articles country (i.e. which country does the article cover)
- `primary_topic_id` - unique identifier of a **primary** topic (i.e. top level). Article can have only a **single** primary topic.

#### article_topic.csv
Here you will find information on articles topics. Columns in `article_topic.csv` are:

- `article_id` - unique article identifier
- `topic_id` - unique topic identifier
- `topic_desc` - topics description/name

#### topic_relationships.csv
Here you will fins hierarchical relationships between differente topics. Columns in `topic_relationships.csv` are:

- `parent_topic_id` - unique identifier of a **parent** topic (i.e. first level). Article can have **multiple** parent topics.
- `child_topic_id` - unique identifier of a **child** topic (i.e. second level). Article can have **multiple** child topics under 

Every Mondaq article can have multiple **parent** topics, where one of those **parent** topics is also chosen to be a **primary** topic. 
For example, let`s say that an article has 3 **parent** topics: "Employment", "Tax" and "Immigration". One of those parent topics is then chosen to be as one single main topic - aka **primary** topic. 