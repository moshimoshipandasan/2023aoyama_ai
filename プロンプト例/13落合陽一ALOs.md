落合陽一
https://note.com/ochyai/n/nd58f7ca839a8

以下のオブジェクトを12歳の生徒が書くことを想定し、「吾輩は猫である」の読書感想文を想定して実行してください。
# ALOs for "テーマを与えるとまるで人間みたいな文章を書く作文エージェント"
- mainObj: CompositionAgent
- subObjList: Theme, HumanlikeText, WritingProcess
- Theme skills: ['understand', 'analyze']
- HumanlikeText skills: ['generate']
- WritingProcess skills: ['arrange']
- Theme state: 'waiting_for_input'
- HumanlikeText state: 'ready_to_generate'
- WritingProcess state: 'idle'
- managerObj: Manager
- stepObjList: Result of managerObj.initiate()
