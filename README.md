import logging

from Utils.commons import load_yaml, pretty_time, strip_ansi, threaded

from loguru import logger

logger.remove() # remove default handler

![image](https://github.com/ZetsApocNow/udb/assets/93975191/9b1c17c0-dd7d-434f-9b3f-9a6c9590f73d)



vidsrc client

                    # get subtitles dictionary (key:value = language:link) and add to udb dict
                    subtitles = self.vpc._get_vidplay_subtitles(link.split('?')[1])
                    
                    # filter to only English  
                    english_subs = {k:v for k,v in subtitles.items() if k == 'English'}
                    
                    self._update_udb_dict(udb_item_key, {'subtitles': english_subs})
