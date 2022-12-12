# xml-to-json
import xmltodict,json
with open('data_l1.xml', 'r') as myfile:
    obj = xmltodict.parse(myfile.read())
print(json.dumps(obj))
print(obj["employees"]["employee"]['name'])
