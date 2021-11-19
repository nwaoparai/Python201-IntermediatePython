from contextlib import contextmanager<br/><br/>


@contextmanager<br/>
def file_open(path):<br/>
    &ensp;try:<br/>
        &ensp;&ensp;f_obj = open(path, 'w')<br/>
        &ensp;&ensp;yield f_obj<br/>
    &ensp;except OSError:<br/>
        &ensp;&ensp;print("We had an error!")<br/>
    &ensp;finally:<br/>
        &ensp;&ensp;print('Closing file')<br/>
        &ensp;&ensp;f_obj.close()<br/><br/>


if &#95;&#95;name&#95;&#95; == '&#95;&#95;main&#95;&#95;':<br/>
    &ensp;with file_open('test.txt') as fobj:<br/>
        &ensp;&ensp;fobj.write('Testing context managers')
