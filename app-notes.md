import pygsheets

gc = pygsheets.authorize() # This will create a link to authorize

# Open spreadsheet
sh = gc.open('google spreadsheet name')

# Open spreadsheet by 'key'

sh = gc.open_by_key('spreadsheet_key')

# Open spreadsheet by 'link'

sh.open_by_link('spreadsheet link')

# Open Worksheet

wk1 = sh[0] # Open first worksheet of spreadsheet
# Or
wk1 = sh.sheet1 # sheet1 is name of first worksheet

"""
    First worksheet has index 0, second had index 1, so on...
    Instead of index, you can use the worksheet name
"""