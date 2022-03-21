# Project4EC530

## Phase 1: Simple queue system using Celery and rabbitmq server
1. Start rabbit server using command sudo rabbitmq-server
2. To see process in action: celery -A queueSystem worker -l INFO 
3. In python interactive shell run:
from queueSystem import add
for i in range(0,1000):
  add.delay(i, i)
