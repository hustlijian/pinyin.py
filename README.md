pinyin.py
=========
source: [clerverdeng/pinyin](https://github.com/cleverdeng/pinyin.py)

汉字转拼音,With Python


Example:

    from pinyin import PinYin
    
    test = PinYin()
    test.load_word()
    string = "一个测试" 
    print "in: %s" % string
    print "out: %s" % str(test.hanzi2pinyin(string=string))
    print "out: %s" % test.hanzi2pinyin_split(string=string, split="-")

    string = "google chrome版本32"
    print "in: %s" % string
    print "out: %s" % str(test.hanzi2pinyin(string=string))
    print "out: %s" % test.hanzi2pinyin_split(string=string, split="-")


Out:
    in: 一个测试
    out: ['yi', 'ge', 'ce', 'shi']
    out: yi-ge-ce-shi
    in: google chrome版本32
    out: [u'g', u'o', u'o', u'g', u'l', u'e', u' ', u'c', u'h', u'r', u'o', u'm', u'e', 'ban', 'ben', u'3', u'2']
    out: g-o-o-g-l-e- -c-h-r-o-m-e-ban-ben-3-2
